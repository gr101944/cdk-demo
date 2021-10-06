# Welcome to your CDK TypeScript project!
cdk init --language=typescript

npm i @aws-cdk/aws-apigateway @aws-cdk/aws-lambda @aws-cdk/aws-codepipeline @aws-cdk/aws-codepipeline-actions @types/aws-lambda @aws-cdk/pipelines

npx cdk bootstrap  --profile default --cloudformation-execution-policies arn:aws:iam::aws:policy/AdministratorAccess aws://accountno/us-east-1

## Note: replace accountno with AWS account number. Bootstrapping needs to be done once per (Account and Region) combination


  
npx cdk deploy --profile default <stack name>
  
## Note: default above is the AWS profile, it may be different and you have to choose what you have in your profile
  

This is a blank project for TypeScript development with CDK.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

## Useful commands

 * `npm run build`   compile typescript to js
 * `npm run watch`   watch for changes and compile
 * `npm run test`    perform the jest unit tests
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk synth`       emits the synthesized CloudFormation template
