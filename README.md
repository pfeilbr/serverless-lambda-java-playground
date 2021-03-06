# serverless-lambda-java-playground

[serverless framework](https://serverless.com/) + [lambda java](https://docs.aws.amazon.com/lambda/latest/dg/java-programming-model.html)

## Build and Deploy

```sh
cd ~/projects/serverless-lambda-java-playground
serverless create --template aws-java-maven
mvn clean install
sls deploy --verbose
sls invoke --function hello --data '{"msg": "hello"}' --log
```

```json
{
    "statusCode": 200,
    "body": "{\"message\":\"Go Serverless v1.x! Your function executed successfully!\",\"input\":{}}",
    "headers": {
        "X-Powered-By": "AWS Lambda & serverless"
    },
    "isBase64Encoded": false
}
```

## Resources

* [How to create a REST API in Java using DynamoDB and Serverless](https://serverless.com/blog/how-to-create-a-rest-api-in-java-using-dynamodb-and-serverless/)