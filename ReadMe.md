## ABOUT

1. This Project is a basic dynamic web aplication which is built on Spring MVC Architecture.
2. This just a practice project from which we can easily understand the flow of data and requests 
   in a Model View Control(MVC) Architecture.
3. Microsoft SQL server is used for database purpose.
4. Stored Procedures are used instead of regular SQL queries from JAVA.
5. All the web pages are downloaded from online resources.
6. All the dependecies of the project are mentioned in pom.xml from line 18 onwards.

## Tools Used

1) Eclipse IDE
2) Apache Tomcat Server 8.0.30
3) Microsoft SQL Server 2014 SP1


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
 1. JAVA 1.7.0 or later
 2. Maven 3.2.0 or later 


## DEPENDENCIES
1. spring-orm-4.3.8.RELEASE
2. spring-beans-4.3.8.RELEASE
3. spring-core-4.3.8.RELEASE
4. spring-tx-4.3.8.RELEASE
5. spring-test-4.3.8.RELEASE
6. spring-jdbc-4.3.8.RELEASE
7. mssql-jdbc-6.1.7.jre8-preview
8. javax.servlet-api-3.1.0
9. jsp-api-2.1
10. jstl-1.2
11. standard-1.1.2
12. junit-4.11
13. hamcrest-core-1.3
14. commons-codec-1.4
15. log4j-1.2.17
16. gson-2.8.1
17. json-20160810
18. commons-fileupload-1.2
19. commons-io-1.4
20. mail-1.4
21. activation-1.1
22. dom4j-1.6
23. xml-apis-1.0.b2
24. poi-3.7
25. poi-ooxml-3.7
26. poi-ooxml-schemas-3.7
27. geronimo-stax-api_1.0_spec-1.0
28. xmlbeans-2.3.0
29. stax-api-1.0.1
30. pdfbox-app-2.0.7
31. pdfbox-2.0.7
32. fontbox-2.0.7
33. commons-logging-1.2
34. hashids-1.0.3
35. commons-net-3.6


