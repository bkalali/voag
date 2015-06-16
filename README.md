<snippet>
<content>
## VOAG Demo project
This project is created to demonstrate some of the MuleSoft functionality and capabilities as follows.

1. There are three use cases: create an order, retrieve an inventory of orders and retrieve an order by order id.  
2. src/main/app/voag-front-end.xml contains front end flows which are designed to expose RAML rest APIs.
3. src/main/app/voag-back-end.xml contains back end flows which are designed to access back-end database using database connector.
4. The rest endpoints are secured by SSL and in memory authentication-manager  
   
 
## Prerequisite
1. It is assumed that you have installed MySql database.
2. You have maven apache-maven-3.1.1 or higher installed.
3. You have used DDL from src/test/resources/order.sql to create an order table. 
4. You have updated your database configuration parameters in src/main/resources/db.properties
5. Postman is used for testing these APIs using 
   userid=voag,
   password=voag

## Build, Install and run
1. > mvn clean install
2. This app tested on mule 3.6.1 EE trail version.  

   
  

## The RAML Rest APIs  
There are three RAML Rest APIs:

1. Create an order   
   POST: https://localhost:8083/api/order
2. Get an order
   GET:https://localhost:8083/api/order/{orderId}
3. Get a list of order inventory
   GET: https://localhost:8083/api/inventory

For more information using these APIs, please see APIKit Console (https://localhost:8083/console/) with details examples and schema.            

</content>
<tabTrigger>readme</tabTrigger>
</snippet> 