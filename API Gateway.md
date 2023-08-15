## Configuring API Gateway
after opening your console
* Click on **Create API**, Scroll down to **REST API** and click on **Build**
* On the choose protocol page, select **REST**
* Under create new API select **New API**. 
* Enter the name of the API and click on **Create API** (we called our **API application-api**)

Now let's create the various endpoints (resources). We will create:

The **health** resource to check the application’s health, 

The **user** resource for all data on a single user 

And the users to query all users.

To create the **endpoints(Resources)**.

At the top click on Actions and click on **Create Resource**
On New child resource box, enter the name of the endpoint and select enable **cors**

![image](https://github.com/Tyannherve11/serverless-crud-with-Lambda-API-gateway-EBS/assets/37128739/f94d5774-644e-414c-921a-70cd2e69a3df)


After creating all the resources next is to create the methods of each resource.

The **health** will have just a **GET** method

The **user** resource will have  **GET**, **PUT**, **POST**, and **DELETE** methods.

The **users** resource will have just a **GET** method. 

To create a method: 

Click on the concerned resource: Let’s click on the resource  **health**  

Then go to actions and click **Create Method**

After saving the method, go ahead and repeat the procedure to create the methods for the other resources.

When done creating the methods: click on the  user resource then on Actions and click on **Enable CORS**. ( also do same for the users resource)

Make sure you select **DEFAULT 5XX**

For Access-Control-Allow-Origin enter ‘*’ to allow all origins and click on **Enable CORS**.

When done an important point is to deploy it, the API

Click on **Actions**

Click on **Deploy API**
On the form that pops up select **New Stage** as Deployment stage
you will be taken to the page containing the API root

Please take note of the API root (URL)  because we will need it in our javascript app is below

 Invoke URL: https://h9j9veohd5.execute-api.us-east-2.amazonaws.com/register
