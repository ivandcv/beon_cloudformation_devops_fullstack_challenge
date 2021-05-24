# BEON FullStack Challenge CloudFormation Stack

This CloudFormation Stack creates the services required for the FullStack Challenge for the BEON account.

# Auto deploy

The stack is set up in a such a way that any time new code is pushed to the production branch, the CodePipeline picks up the change and updates the Lambda for you.

# How to generate the CloudFormation file

This repo was build using the [Grapes Frameworks](https://www.npmjs.com/package/@0x4447/grapes). First you need to install the framework:

```
sudo npm install -g @0x4447/grapes
```

Then, go inside this repo and run this command:

```
grapes -s .
```

This will create a `CloudFormation.json` file in the root dir of the repo which you can upload to AWS.