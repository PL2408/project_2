# Project_2
[Flask_Dashboard](https://lopihara.iplatinum.pro)

This project will be created by learning and implementing CI/CD processes using GITHub Actions

The App Generator project was used as a basis, for which I would like to thank's separately.

Link to the project:
* https://github.com/app-generator/flask-adminlte
* Static Web site located in S3 bucket - secondary endpoint

If web server (EC2) is up, Route53 record points to Web Server with web page marked as Dynamic. 
Otherwise Route53 points to the static web page which is located in S3 Bucket.

Project dedicated to learn DevOps technologies and implement them on real case.

## Features of the project:
1. The infrastructure is described as a code using Terraform
2. Build on a AWS platform
3. The site is launched using Docker based on Nginx image
4. Static Web site works through AWS Cloud Front
5. Jenkins is used as main CI/CD tool

Because of using AWS Free Tier this project has some limitations. 
E.g., Public Subnets where used to avoid additional costs for NAT Gateway.

![architecture diagram](cicd/iac/architecture.drawio.png)