# A Serverless Lambda + API Gateway

This a the way to go with API Gateway, because we can run code on and IDE and test it locally either that code and put it directly online

For the purpose of this, I'm going to use Serverless Tools. This help us create more "Developer Friendly" Experience
for building Apps with API Gateway + Lambda.

It will be great for everyone to go through the documentation and look our to setup Serverless on his own computer.

# File Struture

```
    /src
        /functions // all functions are stored here
        /tests // all the tests for a given function
    /templates
```

# Create a function in CLI

To rapidly bootstrap a function and the test, you can run a cli command given by Serverless

```
serverless create function -f FUNCTION_NAME --handler src/functions/FILE_NAME.FUNCTION_NAME --path src/tests/
```

# Deployment

For now, this a sample auto deploy for a template project, but next step is to deploy our real architecture, which is "Mono Repo". Means that we all have our Functions on the same git repository.

# Helper

If you already setup Serverless on your computer and what to create a function just enter this.

# Good to Know

I have installed a coupled on Node modules, for me to be able to run "API Gateway" Offline and one that dependency
in charge off mocking AWS Endpoint is :

```
aws-sdk-mock
```
