###### API Using Amazon AWS

I have used Amazon AWS to create the RESTful API for this task.

Link to API: https://thzpf4wmki.execute-api.us-west-2.amazonaws.com/Dev/trip-earning

To use this API, the client (like Android Studio) will pass a query with the URL. The API will pass in the query as a JSON object to the Lambda function. The Lambda function will then extract the information provided, and either get an item from the DynamoDB, using the get_item() method, or will add an item to the DynamoDB, using put_item().
