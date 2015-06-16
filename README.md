<snippet>
<content>
## VOAG Demo project
This project is created to demonstrate some of the MuleSoft functionality and capabilities as follows:
1. voag-front-end.xml contains front end flows which used to expose RAML rest services.
2. voag-back-end.xml contains back end flows which used to access back-end database.
3. The rest endpoints are secured by SSL and mule's in memory's authentication-manager   
   
 
## Prerequisite
1. This project assumes that you have installed MySql database
2. You have used DDL from src/test/resources/order.sql to create an order table. 
3. Postman is used for testing these APIs using 
   userid=voag,
   password=voag
  

## The RAML Rest APIs  
There are three RAML Rest APIs:

1. Create an order   
   POST: https://localhost:8083/api/order
2. Get an order
   GET:https://localhost:8083/api/order/{orderId}
3. Get a list of order inventory
   GET: https://localhost:8083/api/inventory

For more information using these APIs, please see APIKit Consoles with details examples and schema.            

</content>
<tabTrigger>readme</tabTrigger>
</snippet> 