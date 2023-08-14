## Setting up IAM role
* Login into your AWS management console and click on Services on the top navbar. 

* From the Services drop-down, scroll down and click on Security, Identity and compliance.  

* On the sidebar scroll down and click on IAM.

* On the page that shows up click on Roles

* Click on Create role

* On the trusted entity type, select AWS service, 

*Scroll down and select Lambda as Use case

* Click on Next. You will be taken to a  page to policies for our IAM role.

We are going to attach two policies:
**CloudWatchFullAccess** for the API request
**AmazonDynamoDBFullAccess** for database access 

After selecting the two policies click on next.

* Enter the role name (in our case it is **serverlessapi-role**)

* Scroll and click on **create role**.

We are done creating the IAM role, we will create a Lambda function for the backend of your API. 
This Lambda function creates, reads, updates, and deletes items from DynamoDB. The 
function uses events from API Gateway to determine how to interact with DynamoDB.
