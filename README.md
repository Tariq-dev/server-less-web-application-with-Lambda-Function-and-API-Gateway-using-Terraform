# Server-less-web-application-with-Lambda-Function-and-API-Gateway-using-Terraform
server less web application with Lambda Function and API Gateway using Terraform

1- Clone this repo and then zip the hello.js file into hello.zip using any zipping software or using CLI and will keep this zip file into the same directory only.

2- Create an S3 bucket from the git bash CLI using the command
# aws s3api create-bucket --bucket=mybucket198745 --region=us-east-1

3- Now, it’s time to upload hello.zip into the S3 bucket we just created. We’ll achieve this using the command
# aws s3 cp hello.zip s3://mybucket198745/hello.zip

4- Open git bash and run terraform init. It will download all the required plugins. Then run terraform apply -auto-approve. It will deploy all the resources into AWS cloud, which we can confirm by opening the AWS console in the browser.

5- After running terraform apply -auto-approve command, there will be a URL present in the CLI which will look like the following 
# https://brqhu55tr8.execute-api.us-east-1.amazonaws.com/test

Now you can see the web page Welcome WorkMotion

![image](https://user-images.githubusercontent.com/57076209/161151433-52679b40-41da-434f-b31a-af94b6cbc45a.png)
