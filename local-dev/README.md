## Locally Development

### 1- target lambda function
```js
// ,.foo.js


exports.handler = function (event, context, callback) {
    console.log('-=-=-=-= peter -=-=-=-=')
    console.log('processing', JSON.stringify(event))
}

```

### 2- serverless.yml

```
service: foo-name
provider:
  name: aws
  runtime: nodejs10.0.0
  region: ap-southeast-1
functions:
  peterLambdaFoo:
    handler: foo.handler
```

### 3 - have `serverless` installed

### 4- Run
```
$ $ serverless invoke local --function peterLambdaFoo -p mockEvent.json
```


## Reference
 - [https://serverless.com/framework/docs/providers/aws/cli-reference/install/](https://serverless.com/framework/docs/providers/aws/cli-reference/install/)