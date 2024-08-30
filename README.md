<h1>Contributor : Priyanka Ghiya </h1>
NOTE: <br>
> <b>Remote Site Setting and Named Credentials are used when we want to hit some external api and get the data inside Salesfroce </b> <br>
> <b>Connected Apps are used when External APIS hits to our Saelsforce Org ie. inside the Apex Class with RestResource and URL Mapping, for performing operations on Salesforce Data.</b> <br>
> For Generating the Access Token, we require the Authentication Parameter for the Third Party System Integration with Our Salesforce System we need the following : <br><br>
1. Username : from the salesforce org we can get. <br>
2. Password : logged in users password. <br>
3.Security Token : we can get from the user icons Setting feature. <br>
It is used when any third party external system wants to access the data from Salesforce, it is append along with the password for security purpose and everytime we reset the org password it is also reset. <br>
4. Consumer Key <br>
5. Secret Key <br>
both of this key we will receive from the connected app, which we have created. <br><br>
> Once we get the Access Token, it will be used to Authorize the Endpoint URL.<br><br>
![alt text](image.png) <br><br>
> In the postman, we will be including these parameters as shown in the img.
but For post url you will need to search for access url in developer guide and replace your url till '.com' <br>
Also, for password parameter, first include the password and after that append the security token.<br>
once,you hit send you will receive the ACCESS TOKEN as shown in the img.<br>
![alt text](image-2.png) <br>

> Copy that access token from postman. <br>
> Get the Endpoint URL ie. anything.com/serives/apexrest/urlmappingName.<br>
> Navigate to postMan, in the header parameter use the Authorization as per the img.<br>
![alt text](image-3.png) <br>
> As value to the Authorization use the 'bearer ', keyword and append the access token generated in the previous post call in postman. Refer image.<br>
![alt text](image-4.png) <br>

> An Apex Class Example for all these procedure using apex code for future refernce.<br>
![alt text](image-5.png) <br>
![alt text](image-6.png) <br>
![alt text](image-7.png) <br>


# sfdc-integration-bootcamp

1. **Salesforce Integration Bootcamp Assignments:** https://bit.ly/3paK9E5
2. **Salesforce Integration Bootcamp Slides:** https://bit.ly/41b6C12
3. **Salesforce Integration Bootcamp Notes:** https://bit.ly/44BeNXp
4. **Salesforce Integration Bootcamp Sheet:** https://bit.ly/3pktVs6

**Session #1: 13th May 2023**
- What is Integration?
- Integration Terminologies 
- What is Webservices?
- JSON Fundamentals using Apex
- REST API Fundamentals - REST Callouts & REST Services using Apex
- Postman Tool Fundamentals

**Session #2: 03rd June 2023**
- Authentication Fundamentals
- Authentication in REST API
- Connected Apps
- Auth Providers
- Username and Password Based Authentication in REST API's
- Named Credentials

**Session #3: TBD**
- Implementation of OAuth 2.0
- Implementation of JWT

**Session #4: TBD**
- Fundamentals of Integration Patterns
- Implementation of Integration Patterns
- Integration Best Practices
- Integration Framework/Integration Design Patterns in Apex

