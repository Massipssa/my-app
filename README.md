# Description

The goal of the present project at the first step, is to develop an ETL based mainly on Spark as background Engine.
The ETL will use a Direct Acyclic Graph to model the different input and output data sources as a workflow.

Once the tool is able to exploit a variety of data sources, the next objectify will be to implement some (most used and 
performances data anonymization algorithms). 

The ETL will use microservice architecture (Be able to develop rapidly new small services, to use other technologies,
and to integrate easily other people with different skills). During the development, we will try to model all tool's 
part using Event-Driven pattern and try to avoid as possible as we can the API pattern. To read more about Event-Driven
Architecture see this [link](https://www.oreilly.com/library/view/software-architecture-patterns/9781491971437/ch02.html). 

At the moment the project is composed of (04) services:
- **gui**: User interface. ***To be developed in Angular (Some small parts are already developed)***
- **etl**: is the core component. It implements (and will) the main algorithms to extract, transform and load data from
  different data sources. ***To develop with Scala***   
- **auth**: the component will allow to secure all the parts of the tool (perform authentication, authorization, offer
  many mechanisms to authenticate, authorize, ...) ***To develop with Java, Spring-boot*** 
- **hdfs**: it allows to access the Hadoop File System (not really important at the present moment) ***To develop with Scala*** 
