# jms-neoload

## Setting Up of JMS in Neoload

JMS (Java Message Service) is a Java-based API that provides a way for applications to communicate with each other asynchronously through a messaging system. It allows applications to send and receive messages between them, without having to know each other's details or location.

JMS is based on a publish-subscribe or point-to-point messaging model, where a sender sends messages to a specific destination (queue or topic) and one or more receivers can consume the messages from the destination. This messaging model enables decoupling of applications, which means that applications can operate independently of each other and communicate only when necessary.

JMS also supports message persistence, which means that messages can be stored in a durable store and retrieved later, ensuring that no messages are lost in case of network failure or system outage. JMS also provides a mechanism for transactions, allowing applications to group multiple JMS operations into a single atomic transaction.

JMS is widely used in enterprise applications for asynchronous messaging, and it is supported by many JMS providers such as Apache ActiveMQ, IBM MQ, and Oracle Advanced Queuing.

> There are two types of messaging domains in JMS.
> - Point-to-Point Messaging Domain
> - Publisher/Subscriber Messaging Domain

> Point-to-Point (PTP) Messaging Domain
> In PTP model, one message is delivered to one receiver only. Here, Queue is used as a message oriented middleware (MOM).
> The Queue is responsible to hold the message until receiver is ready.
> In PTP model, there is no timing dependency between sender and receiver.
 
> Publisher/Subscriber (Pub/Sub) Messaging Domain
> In Pub/Sub model, one message is delivered to all the subscribers. It is like broadcasting. Here, Topic is used as a message oriented middleware that is responsible > to hold and deliver messages.
> In PTP model, there is timing dependency between publisher and subscriber.
 
Before you begin setting up JMS in LoadRunner and Neoload, you will need to ensure that you have the following prerequisites:

- A basic understanding of JMS (Java Messaging Service)

- A working knowledge of Neoload

- Access to the JMS provider you want to test (e.g., Apache ActiveMQ, IBM MQ, Oracle Advanced Queuing)

- JMS client libraries for the JMS provider you want to test

- A Java Development Kit (JDK) installed on your machine

- Knowledge of how to configure JMS client libraries in Neoload

## Tools

To set up JMS in LoadRunner and Neoload, you will need the following tools:

- Neoload 7.6

- JMS client libraries for the JMS provider you want to test

- [jboss-client.jar](https://github.developer.allianz.io/ajin-sudhir/jms-neoload/blob/main/jboss-client.jar)

- A Java Development Kit (JDK) installed on your machine

## Process

The process for setting up JMS in LoadRunner and Neoload involves the following steps:

-	Download the JMS client libraries for the JMS provider you want to test and add them to your LoadRunner or Neoload project.

-	Neoload 7.6 – ``` C:\Program Files\NeoLoad 7.6\extlib ```
 
-	Configure the connection factory, destination, and other JMS-related properties.

  
## Steps

-	Create a script in  Neoload that uses the JMS client libraries to send and receive messages

-	Run the script or scenario to test the JMS provider.

### NeoLoad 7.6
 
1.Connect : Connection Settings for Send Queue
 
2.Queue - Send :  Send Queue
 
3.Queue - Receive :  Send Receive
 
4.Disconnect :  Send Queue
 


 

