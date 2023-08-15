## Creating the Lambda Function
* Sign into the Lambda console
* Click on Create a function. 
* For the Function name, enter **serverless-lambda** or a name of your choice just try to be consistent when naming.
* On the runtime select **python 3.10** or the latest python you have. 
* Under Permissions click on **Change default execution role**.
* Select **Use an existing role**.
* For the Role name, enter the role you created earlier and click on create function. Figure 4 shows the complete setup

![image](https://github.com/Tyannherve11/serverless-crud-with-Lambda-API-gateway-EBS/assets/37128739/905bbf83-92f9-4646-a6e1-5a19d72ce328)

* Now click on **Configuration**. 

* Scroll down and click on edit.

* In the basic settings, **change the time to 1 min** and the **memory to 500MB**, then click on Save

* download the code from github https://github.com/utrains/Serverless-lambda-function/archive/refs/heads/main.zip
* unzip the folder
* Copy the **code** in the **lambda_function.py** using **CTRL+C**
* Click on **Code** and Go to your lambda function clear the code inside and paste the copied code. Use **CTRL +V** to paste.

* Go back to the folder you downloaded
* Copy the code in the **custom_encoder.py**.
* Go to AWS lambda function, right click on the folder on the sidebar, and click on New File.then paste
* click on **Deploy**


We are done creating the lambda function and writing the CRUD code. Next, we will create and configure the API gateway
