##ABOUT

1. This Project is a basic dynamic web aplication which is built on Spring MVC Architecture.
2. This just a practice project from which we can easily understand the flow of data and requests 
   in a Model View Control(MVC) Architecture.
3. Microsoft SQL server is used for database purpose.
4. Stored Procedures are used instead of regular SQL queries from JAVA.
5. All the web pages are downloaded from online resources.
6. All the dependecies of the project are mentioned in pom.xml from line 18 onwards.

##Tools Used

1) Eclipse IDE
2) Apache Tomcat Server 8.0.30
3) Microsoft SQL Server 2014 SP1


## FLOW OF PROGRAM EXECUTION
 a)web.xml is the starting point server initialy search for the request("/" initially) in the web.xml.
 b)the url pattern will be matched and the servlet with the specified name will be searched("spring" here). 
 c)execution goes to the servlet with name where we give our servlet class in web.xml ("dispatcherServlet class" here).
 d)dispatcherServlet class sends the execution to spring-servlet.xml where we give the base package name("com.bank").
 e)the dispatcherServlet class search for controller classes for every request and search the class handling the request.
   package=com.bank.controller
 f)Controller class can be mady by using annotation @controller(import the related package)
 g) Controller class is handling all the Http Requests and sending the to AppDao Class through a service class called AppService.
 h) In AppDao class all the JDBC related code is present.


##Minimum Requirments
 1. JAVA 1.7.0 or later
 2. Maven 3.2.0 or later 


##DEPENDENCIES
spring-orm-4.3.8.RELEASE
spring-beans-4.3.8.RELEASE
spring-core-4.3.8.RELEASE
spring-tx-4.3.8.RELEASE
spring-test-4.3.8.RELEASE
spring-jdbc-4.3.8.RELEASE
mssql-jdbc-6.1.7.jre8-preview
javax.servlet-api-3.1.0
jsp-api-2.1
jstl-1.2
standard-1.1.2
junit-4.11
hamcrest-core-1.3
commons-codec-1.4
log4j-1.2.17
gson-2.8.1
json-20160810
commons-fileupload-1.2
commons-io-1.4
mail-1.4
activation-1.1
dom4j-1.6
xml-apis-1.0.b2
poi-3.7
poi-ooxml-3.7
poi-ooxml-schemas-3.7
geronimo-stax-api_1.0_spec-1.0
xmlbeans-2.3.0
stax-api-1.0.1
pdfbox-app-2.0.7
pdfbox-2.0.7
fontbox-2.0.7
commons-logging-1.2
hashids-1.0.3
commons-net-3.6


