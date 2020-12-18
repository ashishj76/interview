# How are Kubernetes and Docker related?
Docker is an open-source platform used to handle software development. Its main benefit is that it packages the settings and dependencies that the software/application needs to run into a container, which allows for portability and several other advantages. Kubernetes allows for the manual linking and orchestration of several containers, running on multiple hosts that have been created using Docker. 

# What is orchestration when it comes to software and DevOps? 
Orchestration refers to the integration of multiple services that allows them to automate processes or synchronize information in a timely fashion. Say, for example, you have six or seven microservices for an application to run. If you place them in separate containers, this would inevitably create obstacles for communication. Orchestration would help in such a situation by enabling all services in individual containers to work seamlessly to accomplish a single goal. 

# What are the main components of Kubernetes architecture?
There are two primary components: the master node and the worker node. Each of these components has individual components in them.

# What is a node in Kubernetes?
A node is the smallest fundamental unit of computing hardware. It represents a single machine in a cluster, which could be a physical machine in a data center or a virtual machine from a cloud provider. Each machine can substitute any other machine in a Kubernetes cluster. The master in Kubernetes controls the nodes that have containers. 

# What is a pod in Kubernetes?
Pods are high-level structures that wrap one or more containers. This is because containers are not run directly in Kubernetes. Containers in the same pod share a local network and the same resources, allowing them to easily communicate with other containers in the same pod as if they were on the same machine while at the same time maintaining a degree of isolation.

# What is a cluster of containers in Kubernetes? 
A cluster of containers is a set of machine elements that are nodes. Clusters initiate specific routes so that the containers running on the nodes can communicate with each other. In Kubernetes, the container engine (not the server of the Kubernetes API) provides hosting for the API server


# What are Daemon sets?
A Daemon set is a set of pods that runs only once on a host. They are used for host layer attributes like a network or for monitoring a network, which you may not need to run on a host more than once.

# What is ‘Heapster’ in Kubernetes?
A Heapster is a performance monitoring and metrics collection system for data collected by the Kublet. This aggregator is natively supported and runs like any other pod within a Kubernetes cluster, which allows it to discover and query usage data from all nodes within the cluster.

# What is a Namespace in Kubernetes?
Namespaces are used for dividing cluster resources between multiple users. They are meant for environments where there are many users spread across projects or teams and provide a scope of resources.

# Name the initial namespaces from which Kubernetes starts?
Default
Kube – system
Kube – public

# What is the Kubernetes controller manager?
The controller manager is a daemon that is used for embedding core control loops, garbage collection, and Namespace creation. It enables the running of multiple processes on the master node even though they are compiled to run as a single process.

# What are the types of controller managers?
The primary controller managers that can run on the master node are the endpoints controller, service accounts controller, namespace controller, node controller, token controller, and replication controller.

# What are the different services within Kubernetes?
Different types of Kubernetes services include: 

Cluster IP service - The ClusterIP is the default Kubernetes service that provides a service inside a cluster (with no external access) that other apps inside your cluster can access. 

Node Port service - The NodePort service is the most fundamental way to get external traffic directly to your service. It opens a specific port on all Nodes and forwards any traffic sent to this port to the service.

External Name Creation service

Load Balancer service - The LoadBalancer service is used to expose services to the internet. A Network load balancer, for example, creates a single IP address that forwards all traffic to your service.  

# What is Kubelet?
The kubelet is a service agent that controls and maintains a set of pods by watching for pod specs through the Kubernetes API server. It preserves the pod lifecycle by ensuring that a given set of containers are all running as they should. The kubelet runs on each node and enables the communication between the master and slave nodes.

# What is Kubectl?
Kubectl is a CLI (command-line interface) that is used to run commands against Kubernetes clusters. As such, it controls the Kubernetes cluster manager through different create and manage commands on the Kubernetes component

# How can you get a static IP for a Kubernetes load balancer? 
A static IP for the Kubernetes load balancer can be achieved by changing DNS records since the Kubernetes Master can assign a new static IP address.

# What is a sidecar container, and what would you use it for?
A sidecar container is a utility container that is used to extend support for a main container in a Pod. Sidecar containers can be paired with one or more main containers, and they enhance the functionality of those main containers. An example would be using a sidecar container specifically to process system logs or for monitoring.

# How do logs work for pods?
With a traditional server setup, application logs are written to a file and then viewed either on each server or collected by a logging agent and sent to a centralized location. In Kubernetes, however, writing logs to disk from a pod is discouraged since you would then have to manage log files for pods. The better way is to have your application output logs to stdout and stderr. The kubelet on each node collects stdout and stderr on the running pods and then combines them into a log file managed by Kubernetes. Then you can use different kubectl commands to view the logs

# How can you separate resources?
You can separate resources by using namespaces. These can be created either using kubectl or applying a YAML file. After you have created the namespace you can then place resources, or create new resources, within that namespace. Some people think of namespaces in Kubernetes like a virtual cluster in your actual Kubernetes cluster.

