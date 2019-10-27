# serverless-lambda-java-playground

## Build and Deploy

```sh
cd ~/projects/serverless-lambda-java-playground
serverless create --template aws-java-maven
mvn clean install
sls deploy --verbose
sls invoke --function hello
```

## Resources

* [How to create a REST API in Java using DynamoDB and Serverless](https://serverless.com/blog/how-to-create-a-rest-api-in-java-using-dynamodb-and-serverless/)