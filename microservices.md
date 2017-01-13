#Account service:
![Account Service](images/lab6_account1.png "Account Service")
![Account Service](images/lab6_account12.png "Account Service")

#Web service:
![Web Service](images/lab6_web.png "Web Service")
![Web Service](images/lab6_web2.png "Web Service")

#The service registration service has the two microservices registered:
![Registration Service](images/lab6_registration_log.png "Web Service")
![Registered 2 microservices](images/lab6_registration1.png "Registered 2 microservices")

#A second account microservice is running in the port 4444 and it is registered:
![Account Service 2](images/lab6_registration_log2.png "Account Service 2")
![Registered 3 microservices](images/lab6_registration2.png "Registered 3 microservices")

#A brief report describing what happens when you kill the microservice with port 2222. Can the web service provide information about the accounts? Why?
When the Account server in port 2222 is killed and the Web server tries to provide information about the accounts, as its imposible to privide that information it returns a Connection Refused error.
Then it asks the register service in order to obtain a working accounts service, and it responds with the service of port 4444.