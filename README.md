# AWS-SAM_ci-cd

>>>>First please change the parameters values in "parameters.json" file.


#Create AWS cloudformation template using below aws cli command:

Command:

aws cloudformation create-stack --stack-name myteststack --template-body file://codepipeline.yaml --parameters file://parameters.json 

#With the below four stages:

#Picture:

![codepipeline](https://user-images.githubusercontent.com/51155045/126156895-c5b6811f-b8d1-4074-b382-ceb9c99a13fd.PNG)

And two cloudformation stacks will be created as below:

> First Creates Complete Codepipeline {CI/CD}.


> Second creates the serverless lambda function using SAM-template placed in the root directory and API gateway to invoke that lambda.

![lambdastack](https://user-images.githubusercontent.com/51155045/126157041-c56e4fd4-1d95-414d-9875-8b86a95d0fdb.PNG)
