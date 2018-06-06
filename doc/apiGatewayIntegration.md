# Integration of apiGateway and lambda
Using API Gateway stage variables to manage Lambda functions

## Lambda

### Logging

![image](https://user-images.githubusercontent.com/5538753/41021279-6da185d4-6998-11e8-8438-6da1d1e6c5aa.png)

## APIGateway

### Create an APIGateway
In the API Gateway console, create a new API called LambdaVar:

![image](https://s3.amazonaws.com/awscomputeblogmedia/1_API-Gateway-create-new-API.png)

### Deploy a lambda function

![image](https://user-images.githubusercontent.com/5538753/41021369-bedeb4b2-6998-11e8-9cb7-2b50fea2530b.png)

### Setting stageVariable for different env

![image](https://user-images.githubusercontent.com/5538753/41021718-fa9fa0f0-6999-11e8-9457-3239cde80965.png)


### Public URL
![image](https://user-images.githubusercontent.com/5538753/41021521-3fe74b96-6999-11e8-9c9c-2bd85039ec88.png)

## Testing 

### Test apiGateway
open 
 - [https://5m86ho2m7l.execute-api.ap-southeast-1.amazonaws.com/dev?name=peter&id=myid](https://5m86ho2m7l.execute-api.ap-southeast-1.amazonaws.com/dev?name=peter&id=myid) 
 
 in browser, with query string `id` and `name`

### See Loggin
![image](https://user-images.githubusercontent.com/5538753/41021660-c9a29912-6999-11e8-9d63-6b7603bfa5ed.png)




## Reference
 - [https://aws.amazon.com/blogs/compute/using-api-gateway-stage-variables-to-manage-lambda-functions/](https://aws.amazon.com/blogs/compute/using-api-gateway-stage-variables-to-manage-lambda-functions/)