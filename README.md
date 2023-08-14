# serverless-crud-with-Lambda-API-gateway-EBS
Build a user registration API with API Gateway, Lambda and DynamoDB


You are the team head in charge of a project to register employees in your company. Given that this project involves registering users and searching for various users, launching an entire server for this will be of great loss to the company. So your task here is to look for the possible solution that won’t involve launching a whole server thereby reducing cost. After doing some research and discussing with the developers, you decided to go servers. 

In the Serverless solution:

* The front end app was built completely with JavaScript, HTML, css and hosted on an s3 bucket. ( this is done by the developers)
* The backend was coded as a lambda function
* The data was transferred from the front end  to the backend using an  API gateway and finally you used DynamoDB to save your data.

In other to  do this  you used the following services

**Services to be used**
– AWS Lambda
– AWS API Gateway
– Dynamodb
– Amazon S3
– Amazon CloudFront
– Amazon Route 53
– AWS Certificate Manager
