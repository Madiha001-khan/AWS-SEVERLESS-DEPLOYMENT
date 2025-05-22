# AWS-SEVERLESS-DEPLOYMENT
A serverless application to manage student details, built with AWS Lambda, API Gateway, and DynamoDB. 
This project follows a fully serverless architecture, enabling cost-efficient, scalable, and easily deployable backend services.

# How It Works:
1)API Gateway receives a POST request.
2)Lambda Function (insertStudentData.py) is triggered.
3)DynamoDB Table (StudentData) stores the student details.

# ARCHITECTURE DIAGRAM:
![image alt](https://raw.githubusercontent.com/Madiha001-khan/AWS-SEVERLESS-DEPLOYMENT/8d7578f0a5ad536875fc2f9975bbab7805884055/image.jpg.png)

# Tech Stack
1)AWS Lambda
2)Amazon API Gateway
3)Amazon DynamoDB
4)AWS IAM
5)AWS SAM / Serverless Framework (for deployment)
6)Python 3.12/ Python (customizable based on language used)

# Benefits of This Serverless Approach
1)Low maintenance – No servers to patch or manage
2)Auto-scaling – Automatically handles more traffic
3)Pay-as-you-go – Cost-effective pricing model
4)Modular & extensible – Easy to expand with new features 
