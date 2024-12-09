# Welcome to your CDK JavaScript project

This is a blank project for CDK development with JavaScript.

The `cdk.json` file tells the CDK Toolkit how to execute your app. The build step is not required when using JavaScript.

## Useful commands

* `npm run test`         perform the jest unit tests
* `npx cdk deploy`       deploy this stack to your default AWS account/region
* `npx cdk diff`         compare deployed stack with current state
* `npx cdk synth`        emits the synthesized CloudFormation template

## Architecture Diagram

```plaintext
+---------------------+
|    S3 Bucket        |
|  (Image Storage)    |
+----------+----------+
           |
           v
+----------+----------+
|    AWS Lambda       |
|  (Image Processing) |
+----------+----------+
           |
           v
+----------+----------+
|  DynamoDB Table     |
| (Image Labels Store)|
+---------------------+