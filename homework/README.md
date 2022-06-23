# Steps for the homework
- Install NodeJs version 14
- Install Serverless framework: https://www.serverless.com/framework/docs/getting-started (Ignore all the possible outputs)
- Create an IAM user in AWS console and grant Administrator access (!!! IMPORTANT !!! This is a bad practice and made so just to keep the example simple.)
- Configure an AWS profile in ~/.aws/credentials
- Head to /homework folder
- Create a "resize-bucket" in S3
- Update serveless.yml with your configuration
- Run npm i
- Run sls deploy

# Test
- Head to "upload S3 bucket"
- Upload a png image
- See the result in "result bucket"
- Examine Cloud Formation Stack
- How many resources were created under the hood ?
- Head to CloudWatch
- Find and examine lambda execution logs
- Try to modify "index.js" code and redeploy the project
- Try to modify "serverless.yml" (e.g.: set different values to RESIZE_WIDTH variable)

# Clean up
- Run sls remove
- Delete the IAM user created for this lab