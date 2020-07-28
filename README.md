# API Using Amazon AWS

I have used Amazon AWS to create the RESTful API for this task.

Link to API: https://thzpf4wmki.execute-api.us-west-2.amazonaws.com/Dev/trip-earning

To use this API, the client (like Android Studio) will pass a query with the URL. The API will pass in the query as a JSON object to the Lambda function. The Lambda function will then extract the information provided, and either get an item from the DynamoDB, using the get_item() method, or will add an item to the DynamoDB, using put_item().

I have added the code of the Lambda function in the repository. I have two lambda functions: AddTripEarning (for adding a new item to the DynamoDB) and GetTripByID(for getting the item from the DynamoDB)


### The get_item() test response from API:

![](https://github.com/navgarg/UI_App_API/blob/master/Images/Screenshot%202020-07-28%20at%2010.44.19%20AM.png)


### The put_item() test response from API:

![](https://github.com/navgarg/UI_App_API/blob/master/Images/Screenshot%202020-07-28%20at%2010.48.50%20AM.png)

### DynamoDB screenshot:

![](https://github.com/navgarg/UI_App_API/blob/master/Images/Screenshot%202020-07-28%20at%2010.51.11%20AM.png)

