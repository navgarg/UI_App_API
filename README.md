# API Using Amazon AWS

I have used Amazon AWS to create the RESTful API for this task.

Link to API: https://thzpf4wmki.execute-api.us-west-2.amazonaws.com/Dev/trip-earning
(Clicking on the above link throws an error as no query parameter is passed)

To use this API, the client (like Android app) will hit the API with a query. The API will pass the query as a JSON object to the AWS Lambda function, created specifically for accessing the DynamoDB database. Since this Lambda function has been assigned the rights to access and modify the DynamoDB, it will extract the information provided, and either get an item from the DynamoDB, using the get_item() method, or will add an item to the DynamoDB, using put_item().

I have added the code of the Lambda function in the repository. I have two lambda functions: 
1. AddTripEarning (for adding a new item to the DynamoDB), and 
2. GetTripByID(for getting the item from the DynamoDB)

#### The get_item() test response from API:
![](https://github.com/navgarg/UI_App_API/blob/master/Images/Screenshot%202020-07-28%20at%2010.44.19%20AM.png)
#### The put_item() test response from API:
![](https://github.com/navgarg/UI_App_API/blob/master/Images/Screenshot%202020-07-28%20at%2010.48.50%20AM.png)
#### DynamoDB screenshot:
![](https://github.com/navgarg/UI_App_API/blob/master/Images/Screenshot%202020-07-28%20at%2010.51.11%20AM.png)
#### Response from API in browser 
Using URL https://thzpf4wmki.execute-api.us-west-2.amazonaws.com/Dev/trip-earning?Trip_ID=1
![](https://github.com/navgarg/UI_App_API/blob/master/Images/Screenshot%202020-07-28%20at%2010.58.31%20AM.png)
