## OPMAlerts

### Introduction
    TicketService is a demo web application to book concert tickets. 
    Its a simple fun application to demostrate security features of AWS Cognito. 
    
    AWS Cognito is used for Access control, sign-in and sign-up for the web application.
    
    Specifically AWS Cognito is used for -
    -   Identity Federation : Users can sign in through identity providers like Google and Amazon.
    -   Cognito User Pools : Users can create their identity in the secure user directory.
    
    In addition this application lets users reset their passwords.
___________________________________________________________________________________________________

### Hosting
##### This website is hosted on AWS S3 @ [TicketService](http://ticketservice-20190327092338-hostingbucket-prod.s3-website-us-east-1.amazonaws.com/)
___________________________________________________________________________________________________

### Technical Components
   
- Framework      : [AWS Amplify](https://aws-amplify.github.io/)<br>
- UI             : React<br>
- AuthN/AuthZ    : Cognito User Pool and Identity Federation from Amazon/Google<br>
- GraphQL        : CRUD operations<br>
- CloudFormation : Infrastructure<br>

___________________________________________________________________________________________________

### Architecture
![Architecture](ticketservice/CognitoArchitecture.png)
