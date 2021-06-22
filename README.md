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
    This source code is packaged and deployed on AWS Lambda.

    The OPM Alerts folder inside of the resources folder in src contains 
    the code for the website, and is uploaded onto an AWS S3 bucket.

    An API Gateway was made to invoke the lambda function when the button on the website is pressed

    A CloudFront Distribution is used to provide a single HTTPS endpoint to
    the backend.

    Route 53 is used to point opm.amoghghadge.com to the CloudFront Distribution

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
