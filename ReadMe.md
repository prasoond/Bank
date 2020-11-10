## ABOUT

1. This Project is a basic dynamic web aplication which is built on Spring MVC Architecture.
2. This just a practice project from which we can easily understand the flow of data and requests 
   in a Model View Control(MVC) Architecture.
3. Microsoft SQL server is used for database purpose.
4. Stored Procedures are used instead of regular SQL queries from JAVA.
5. All the web pages are downloaded from online resources.
6. All the dependecies of the project are mentioned in pom.xml from line 18 onwards.

## Prereuisites

* [Eclipse IDE](https://www.eclipse.org/downloads/) (version 2019-03 (4.11.0) Preferred)
* [Microsoft SQL Server 2014 Management Studio](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15)
* [JAVA 8](https://www.oracle.com/in/java/technologies/javase/javase-jdk8-downloads.html) SDK/JRE
* [Apache Tomcat Server](https://tomcat.apache.org/download-90.cgi)

* Download and Install Microsoft SQL Server 2014 Management Studio and Create table ad insert the mock data form bank/database/Tables foder.

* Change the Microsoft SQL Server 2014 Management Studio login credentials in jdbc.properties file.

* Inside Microsoft SQL Server 2014 Management Studio, after creating database table, go to Programmability/Stored Procedures, Create a Stored Procedure and copy-paste the queries from the bank/Database/Stored Procedure folder.

* Clone/pull the project to your local system.

* Download the Ecilipse IDE, Import the Project in Ecilipse IDE.

* In src/Mail, go to the SendMail.java and update the emailId and password.

* Download Apache Tomcat and Run the Project on Apache Tomcat Server. 



## FLOW OF PROGRAM EXECUTION
 1. web.xml is the starting point server initialy search for the request("/" initially) in the web.xml. 
 2. The url pattern will be matched and the servlet with the specified name will be searched("spring" here).  
 3. Execution goes to the servlet with name where we give our servlet class in web.xml ("dispatcherServlet class" here). 
 4. dispatcherServlet class sends the execution to spring-servlet.xml where we give the base package name("com.bank").
 5. The dispatcherServlet class search for controller classes for every request and search the class handling the request.
    package=com.bank.controller
 6. Controller class can be mady by using annotation @controller(import the related package)
 7. Controller class is handling all the Http Requests and sending the to AppDao Class through a service class called AppService.
 8. In AppDao class all the JDBC related code is present.



## Minimum Requirments
 * JAVA 1.7.0 or later
 * Maven 3.2.0 or later 
 * Apache Tomcat Server 8.0.3 or later
 * Microsoft SQL Server 2014 Management Studio 18.7.1 or later


