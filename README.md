# aws-lambda-nodejs

 Testing AWS Lambda deployment flow(using **Nodejs** and npm package **serverless**).

 Run functions on local machine(local host) using **serverless-offline**.

## Installation

### Step 1
Install serverless on global environment.
```
npm install -g serverless
```

### Step 2
Install package dependencies.
```
npm install –production
```
If trying to run functions on local machine, remember to install dev dependencies.

`npm install` or `npm install --only=dev`

## Usage

### Deployment
In your project root run:
```
serverless deploy --stage {stage}
```
Remember to change `{stage}` to your target environment.

*See Serverless [Github](https://github.com/serverless/serverless) or [Website](https://serverless.com/) for more information.*

### Local Testing
In your project root run:
```
serverless offline
```
*See more options on Serverless-Offline [Github](https://github.com/dherault/serverless-offline)*

And then access `http://localhost:9999` on your browser or api testing tool(like [Postman](https://www.getpostman.com/)).
