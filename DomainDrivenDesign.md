# Useful Links
https://towardsdatascience.com/what-is-domain-driven-design-5ea1e98285e4

# What is a “Domain”?
The subject area on which the application that is being developed applies is called the Domain. When developing an application it is always good to know the context in which it applies. Sometimes there are multiple domains in which an organization can be active. For example, a company can be active in sales, transport and repairs, all at the same time.
An organisation can organise itself differently for sub-domains. If you are developing an application for sales, it is best to look at it from “sales”. The language of the developed application will be aligned with the business and the application will make more sense overall.

# What is a “Bounded context”?
In Domain-Driven Development “Bounded Context” is an important concept. It gives more information on how to deal with large domain models and a large organization. To deal with a large model you can divide the model into different zones which we call a “Bounded Context”.
An organization can be split into a sales department and a support department, each operating within its context. By working in a bounded or limited context the work becomes easier and better organized .

# What does “Ubiquitous Language” mean?
In basic terms, a ubiquitous language is a language shared by the development team and the domain experts. Because they have to work closely together to create a short feedback loop, this makes perfect sense.
The language has to be used not only in the domain model, but also in the code of the application. If the development team and the business team wouldn’t work together, the chance would increase they’d develop their language.
Let’s summarize some key characteristics of the ubiquitous language:
- must be expressed in the Domain Model.
- keeps “technical” developer language out of the Domain Model, which would not be understood by the domain experts.
- mitigates contradictions and inaccuracies to be introduced to the Domain Model by domain experts.
- evolves as the application grows.

# What is an “Anti Corruption Layer”?
To prevent two domains to pollute each other, you have to create a boundary between them. Each domain has its ubiquitous language and its domain model.
An anti-corruption layer translates between the two domain models. The layer can be uni or bi-directional and is often implemented by well-known patterns (e.g. adapter, facade, translator). We have to keep in mind that creating an anti-corruption layer can be time-consuming. It should only be used if you want to protect your domain from outer influences.

# What is the difference between an “Entity” and a “Value Object”?
It’s important to understand the difference between Entities and Value Objects to model the real world in an application. I will list the main differences between them here.
- Identity: Value Objects have no identity, while an Entity does. Value Objects that have the same values are inherently equal. Entities exist on their own.
- Life cycle: Value Objects do not live on their own and belong to some Entity. They can be destroyed and created with ease. Entities live on and have history.

# What is an “Aggregate”?
An aggregate is a domain-driven design pattern. It’s a cluster of domain objects (e.g. entity, value object), treated as one single unit. A car is a good example. It consists of wheels, lights and an engine. They conceptually belong together.
Every aggregate has an aggregate root. In our example, this might be the chassis number. It ensures the integrity of the aggregate as a whole. Every aggregate denotes a transactional boundary