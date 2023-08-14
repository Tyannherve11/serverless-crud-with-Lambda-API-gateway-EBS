We use a DynamoDB table to store data for the App.
Each item has a unique ID, which we use as the partition key for the table.

To create a DynamoDB table
* Open the DynamoDB console
* Choose **create table**
* For table name, enter **_userseverless_**
* For partition key, enter id and allow the data type as string.
* Choose create
