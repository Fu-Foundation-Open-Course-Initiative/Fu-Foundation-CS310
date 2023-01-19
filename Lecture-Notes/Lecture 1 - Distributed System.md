# Lecture 1 - Distributed System

# Fallacies of Distributed Systems

There are several fallacies of distributed systems that are commonly encountered when designing and implementing distributed systems. These include:

1. The network is reliable: This fallacy assumes that the network is always available and that packets are never lost or delayed. In reality, networks can experience outages and congestion, leading to packet loss and delays.
2. Latency is zero: This fallacy assumes that the delay between two machines communicating over a network is zero. In reality, network latency can vary widely depending on factors such as network congestion and the distance between the machines.
3. Bandwidth is infinite: This fallacy assumes that the amount of data that can be transferred over a network is unlimited. In reality, networks have finite bandwidth, and this can be a bottleneck for distributed systems.
4. The network is secure: This fallacy assumes that the network is invulnerable to attacks and that data transmitted over it is always secure. In reality, networks can be vulnerable to a wide range of security threats, such as hacking and eavesdropping.
5. Topology doesn't change: This fallacy assumes that the network topology will remain constant, but in reality, networks are dynamic and the topology can change at any time.
6. There is one administrator: This fallacy assumes that there is a central point of control and administration for the entire system. In reality, distributed systems are typically managed by multiple individuals or organizations.

# Distributed System Characteristics

Distributed systems have a number of unique characteristics that differentiate them from traditional, centralized systems. These include:

1. Concurrency: Distributed systems involve multiple independent processes running simultaneously on different machines.
2. No global clock: Distributed systems do not have a single, global clock that all machines can synchronize to.
    1. This means that timekeeping in a distributed system can be more challenging.
3. Failure handling: Distributed systems are subject to a wide range of failures, including hardware failures, network failures, and software bugs.
    1. The system must be designed to handle these failures and continue to operate in a degraded state if necessary.
4. **Transparency: Distributed systems should hide the complexity of their underlying distribution from the users, making them appear as a single, unified system.**
5. **Scalability: Distributed systems should be designed to be able to handle an increasing number of users and workloads without a significant decline in performance.**
6. Location transparency: Users should not be aware of the location of the resources they are accessing, this will simplify the system design, and make it more flexible.
7. Security: Distributed systems must be designed to protect against unauthorized access and protect the integrity and confidentiality of data.
8. Heterogeneity: Distributed systems often consist of a variety of different hardware and software platforms, making it necessary to design for compatibility and interoperability.

# Distributed System Communication

Communication is a crucial aspect of distributed systems, as it allows different machines and processes to exchange information and coordinate their actions. There are several key types of communication used in distributed systems, including:

1. Remote Procedure Calls (RPCs): This type of communication allows a process on one machine to invoke a procedure or function on another machine.
    1.  The remote procedure call is handled by the operating system or a specialized library, and appears to the calling process as if the procedure were local.
2. Message Passing: This type of communication allows processes to send messages to each other. These messages can be sent using a variety of different protocols, such as TCP/IP or UDP.
3. Publish-Subscribe: This type of communication allows processes to subscribe to a particular topic or channel, and then receive notifications or updates when new information is published on that topic or channel.
4. Shared Memory: This type of communication allows processes to share a common area of memory, allowing them to read and write to it. This is typically used for inter-process communication on a single machine.
5. Object-Oriented Middleware: This type of communication allows objects on different machines to interact with each other as if they were on the same machine, through the use of Remote Method Invocation (RMI) or Common Object Request Broker Architecture (CORBA).

# Benefits of Distributed System

1. Scalability: Distributed systems can be scaled horizontally by adding more machines to the system, which allows for increased capacity and performance.
2. Reliability: Distributed systems can provide redundancy by replicating data and services across multiple machines, which can improve system availability and fault tolerance.
3. Flexibility: Distributed systems can be composed of different types of machines and can run on a variety of platforms, which allows for greater flexibility in the deployment and management of the system.
4. Improved resource utilization: Distributed systems can make more efficient use of resources by distributing workloads across multiple machines, which can lead to cost savings and improved performance.
5. Easy to add new functionality: Distributed systems are easy to extend and add new functionality to, as new services can be added to the system without disrupting existing services.
