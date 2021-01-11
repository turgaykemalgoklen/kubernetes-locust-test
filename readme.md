# Kubernetes Distrubeted Locust Test

This project contains source code and supporting files for the k8s locust test application/yaml files that I created.

This project includes the following files and folders:

- docker - Code for the application's Lambda function.
- events - Invocation events that you can use to invoke the function.
- \_\_tests__ - Unit tests for the application code.
- template.yml - A SAM template that defines the application's AWS resources.
- buildspec.yml -  A build specification file that tells AWS CodeBuild how to create a deployment package for the function.




## Core Services
1. Lambda for trigger API
2. API Gateway for API management
3. DynamoDB for save ID,FirstName,LastName parameters
4. CloudFormation for provisining Infastructure as Code(IaC)
5. CodeCommit&CodeStar&AWS CodePipeline for managining versions&Github repo creation.



## Try the application out

The  application creates a RESTful API that takes HTTP requests and invokes Lambda functions. The API has POST and GET methods on the root path to create and list items. It has a GET method that takes an ID path parameter to retrieve items. Each method maps to one of the application's three Lambda functions.


