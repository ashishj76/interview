# https://natrajbontha.wordpress.com/2019/08/22/c-interview-questions/

# What are the different types of instances?
	Following are the types of instances:
	General purpose
	Computer Optimized
	Memory Optimized
	Storage Optimized
	Accelerated Computing
	
# Explain default storage class in S3
	The default storage class is a Standard frequently accessed.

# Name the types of AMI provided by AWS
The types of AMI provided by AWS are:
	Instance store backed
	EBS backed

# List different types of cloud services
Various types of cloud services are:
	Software as a Service (SaaS),
	Data as a Service (DaaS)
	Platform as a Service (PaaS)
	Infrastructure as a Service (IaaS).	

# What are the different types of Load Balancer in AWS services?
Two types of Load balancer are:
	Network Loab Balanacer
	Application Load Balancer
	Classic Load Balancer
	
# Common Question
---------------
# Solid principles
- (S) Single Responsiblity. A class should have one and only one reason to change, meaning that a class should have only one job.
- (O) Open Closed principle. Objects or entities should be open for extension, but closed for modification.
- (L) Liskov substitution principle
- (I) Interface segregation principle. A client should never be forced to implement an interface that it doesn't use or clients shouldn't be forced to depend on methods they do not use.
- (D) Dependency Inversion Principle. Decoupling. Entities must depend on abstractions not on concretions. It states that the high level module must not depend on the low level module, but they should depend on abstractions.

What are microservices?
Microservices - also known as the microservice architecture - is an architectural style that structures an application as a collection of services that are
- Highly maintainable and testable
- Loosely coupled
- Independently deployable
- Organized around business capabilities
- Owned by a small team

What is the difference between Monolithic, SOA and Microservices Architecture? What is the difference between Monolithic, SOA and Microservices Architecture?
- Monolithic Architecture is similar to a big container wherein all the software components of an application are assembled together and tightly packaged.
- A Service-Oriented Architecture is a collection of services which communicate with each other. The communication can involve either simple data passing or it could involve two or more services coordinating some activity.
- Microservice Architecture is an architectural style that structures an application as a collection of small autonomous services, modeled around a business domain.

What are main differences between Microservices and Monolithic Architecture? What are main differences between Microservices and Monolithic Architecture?

- Microservices
	- Service Startup is fast
	- Microservices are loosely coupled architecture.
	- Changes done in a single data model does not affect other Microservices.
	- Microservices focuses on products, not projects
- Monolithic Architecture
	- Service startup takes time
	- Monolithic architecture is mostly tightly coupled.
	- Any changes in the data model affect the entire database
	- Monolithic put emphasize over the whole project

# .NET Core
------------

# What are some characteristics/features of .NET Core?

- Flexible deployment: Can be included in your app or installed side-by-side user- or machine-wide.
- Cross-platform: Runs on Windows, macOS and Linux; can be ported to other OSes. The supported Operating Systems (OS), CPUs and application scenarios will grow over time, provided by Microsoft, other companies, and individuals.
- Command-line tools: All product scenarios can be exercised at the command-line.
- Compatible: .NET Core is compatible with .NET Framework, Xamarin and Mono, via the .NET Standard Library.
- Open source: The .NET Core platform is open source, using MIT and Apache 2 licenses. Documentation is licensed under CC-BY. .NET Core is a .NET Foundation project.
- Supported by Microsoft: .NET Core is supported by Microsoft, per .NET Core Support

# What's the difference between SDK and Runtime in .NET Core?
- The SDK is all of the stuff that is needed/makes developing a .NET Core application easier, such as the CLI and a compiler.
- The runtime is the "virtual machine" that hosts/runs the application and abstracts all the interaction with the base operating system.

# What is difference between .NET Core and .NET Framework?
.NET as whole now has 2 flavors:
	- .NET Framework
	- .NET Core
.NET Core and the .NET Framework have (for the most part) a subset-superset relationship. .NET Core is named “Core” since it contains the core features from the .NET Framework, for both the runtime and 
framework libraries. For example, .NET Core and the .NET Framework share the GC, the JIT and types such as String and List. .NET Core was created so that .NET could be open source, cross platform and be used 
in more resource-constrained environments.

# Explain what is included in .NET Core?	
- A .NET runtime, which provides a type system, assembly loading, a garbage collector, native interop and other basic services.
- A set of framework libraries, which provide primitive data types, app composition types and fundamental utilities.
- A set of SDK tools and language compilers that enable the base developer experience, available in the .NET Core SDK.
- The 'dotnet' app host, which is used to launch .NET Core apps. It selects the runtime and hosts the runtime, provides an assembly loading policy and launches the app. 
The same host is also used to launch SDK tools in much the same way.

# What's the difference between .NET Core, .NET Framework, and Xamarin?
- .NET Framework is the "full" or "traditional" flavor of .NET that's distributed with Windows. Use this when you are building a desktop Windows or UWP app, or working with older ASP.NET 4.6+.
- .NET Core is cross-platform .NET that runs on Windows, Mac, and Linux. Use this when you want to build console or web apps that can run on any platform, including inside Docker containers. This does not include UWP/desktop apps currently.
- Xamarin is used for building mobile apps that can run on iOS, Android, or Windows Phone devices.

# What is CoreCLR?
CoreCLR is the .NET execution engine in .NET Core, performing functions such as garbage collection and compilation to machine code.

# Explain the difference between Task and Thread in .NET
Thread: Thread is the means by which you can get the task done. It represents actually at OS level thread, with its own stack and kernel. With threads you can Abort, suspend, resume, observe state. ThreadPool is the wrapper around pools of thread manitained by CLR.
Task: Task is something you need to get done. 
In .NET 4.0 terms, a Task represents an asynchronous operation. Thread(s) are used to complete that operation by breaking the work up into chunks and assigning to separate threads.

# What are the benefits of explicit compilation?
Ahead of time (AOT) delivers faster start-up time, especially in large applications where much code executes on startup. But it requires more disk space and more memory/virtual address space to keep both the IL and precompiled images. In this case the JIT Compiler has to do a lot of disk I/O actions, which are quite expensive.

# What is the use of ConfigureServices method of startup class?
This is an optional method of startup class. It can be used to configure the services that are used by the application. This method calls first when the application is requested for the first time. Using this method, we can add the services to the DI container, so services are available as a dependency in controller constructor.

# What is the use of the Configure method of startup class?
It defines how the application will respond to each HTTP request. We can configure the request pipeline by configuring the middleware. It accepts IApplicationBuilder as a parameter and also it has two optional parameters: IHostingEnvironment and ILoggerFactory. Using this method, we can configure built-in middleware such as routing, authentication, session, etc. as well as third-party middleware.

# What is routing in ASP.NET Core?
Routing is functionality that map incoming request to the route handler. The route can have values (extract them from URL) that used to process the request. Using the route, routing can find route handler based on URL. All the routes are registered when the application is started. There are two types of routing supported by ASP.NET Core
	-	The conventional routing
	-	Attribute routing
	
# What are the various JSON files available in ASP.NET Core?
There are following JSON files in ASP.NET Core :
	-	global.json
	-	launchsettings.json
	-	appsettings.json
	-	bundleconfig.json
	-	bower.json
	-	package.json

# How to specify service lifetime for register service that added as a dependency?
- Singleton. .NET core  will create and share a single instance of the service through the application life.Objects are the same for every object and every request.
- Transient are always different; a new instance is provided to every controller and every service.
- Scoped Scoped objects are the same within a request, but different across different requests.

# What are the drawbacks of using a singleton design pattern?
The major drawbacks of using a singleton design pattern are:
a)Singleton causes code to be tightly coupled. The singleton object is exposed globally and is available to a whole application. Thus, classes using this object become tightly coupled; any change in the global object will impact all other classes using it.
b)They hide dependencies instead of exposing them.
c)Singleton Pattern does not support inheritance.
d)Singleton principle can be violated by techniques such as cloning. If an application is running on multiple JVM’s, then, in this case, Singleton might be broken.

# Why use a factory class to instantiate a class when we can use a new operator?
Factory classes provide flexibility in terms of design. Below are some of the benefits of factory class:
•Factory design pattern results in more decoupled code as it allows us to hide creational logic from dependant code
•It allows us to introduce an Inversion of Control container
•It gives you a lot more flexibility when it comes time to change the application as our creational logic is hidden from dependant code
