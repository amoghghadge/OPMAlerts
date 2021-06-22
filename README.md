## OPMAlerts

### Introduction
    TicketService is a demo web application to book concert tickets. 
    Its a simple fun application to demostrate security features of AWS Cognito. 
    
    AWS Cognito is used for Access control, sign-in and sign-up for the web application.
    
    Specifically AWS Cognito is used for -
    -   Identity Federation : Users can sign in through identity providers like Google and Amazon.
    -   Cognito User Pools : Users can create their identity in the secure user directory.
    
    In addition this application lets users reset their passwords.

    The website is opm.amoghghadge.com
___________________________________________________________________________________________________

### Hosting
##### This source code is packaged and deployed on AWS Lambda.

##### The OPM Alerts folder inside of the resources folder in src contains 
##### the code for the website, and is uploaded onto an AWS S3 bucket.

___________________________________________________________________________________________________

### Technical Components
   
- Source Code            : Packaged and deployed on AWS Lambda<br>
- Website                : Uploaded to an S3 bucket<br>
- API                    : API Gateway invokes the lambda function when the button on the website is pressed<br>
- Application Endpoint   : CloudFront provides an HTTPS endpoint to the backend<br>
- DNS                    : Route 53 points opm.amoghghadge.com to the CloudFront Distribution<br>

___________________________________________________________________________________________________

### Architecture
![Architecture](ticketservice/CognitoArchitecture.png)
