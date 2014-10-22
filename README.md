Apigee4g
========
The proxies can be deployed by switching to the APIs directory which is located in the proxies directory (e.g. cd proxies/organizations)
Then following the steps outlined below.  


**Deployment using maven**


*Pre-requisite*

1. Java(TM) SE Runtime Environment 1.6 or later
2. Apache Maven 3.0.3 or later [Download](http://maven.apache.org/download.cgi)
3. Access to On-Premise (4G) environment over HTTP


*Maven Commands*

- cd {project folder}  (eg. cd native-mobile-service)

- Deploy Commands

  *Standard Deployment* 
  ``` 
  mvn apigee-enterprise:deploy -P{profile-id} –Dusername={apigee login} -Dpassword={apigee password}
  ```
  where profile-id is one of - dev,stage,cert,prod


  *clean deployment* 
  ```  
  mvn apigee-enterprise:deploy -P{profile-id} -Dapigee.options=clean –Dusername={apigee login} -Dpassword={apigee password}
  ```
  This will undeploy and delete the current version before deploying the new build


  
*Shell Command
To deploy the bundle execute the following commands.

cd {project folder}  (eg. cd native-mobile-service)

./deploy.sh test user@email.com password



