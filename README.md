# AWS-SERVERLESS-DEPLOYMENT
A serverless application to manage student details, built with AWS Lambda, API Gateway, and DynamoDB. 
This project follows a fully serverless architecture, enabling cost-efficient, scalable, and easily deployable backend services.

# How It Works:
1)API Gateway receives a POST request.
2)Lambda Function (insertStudentData.py) is triggered.
3)DynamoDB Table (StudentData) stores the student details.

# ARCHITECTURE DIAGRAM:
![image alt](https://raw.githubusercontent.com/Madiha001-khan/AWS-SEVERLESS-DEPLOYMENT/8d7578f0a5ad536875fc2f9975bbab7805884055/image.jpg.png)

# TECH STACK:
1)AWS Lambda
2)Amazon API Gateway
3)Amazon DynamoDB
4)AWS IAM
5)AWS SAM / Serverless Framework (for deployment)
6)Python 3.12/ Python (customizable based on language used)

# BENEFITS:
1)Low maintenance – No servers to patch or manage
2)Auto-scaling – Automatically handles more traffic
3)Pay-as-you-go – Cost-effective pricing model
4)Modular & extensible – Easy to expand with new features 

# DEPLOYMENT STEPS:
   ## 1)Create a DynamoDB Table
     i)Table Name: StudentRecords
     ii)Primary Key: student_id (String)

## 2)Write Lambda Functions
     i)addStudent – Add new student data.
     ii)getStudent – Retrieve student info by ID.
     iii)updateStudent – Modify existing data.
     iv)deleteStudent – Remove a student record.

## 3)Deploy Lambda Functions
     i)Use AWS CLI or AWS Console.
     ii)Grant appropriate execution roles with DynamoDB access.

## 4)Configure API Gateway
    i)Create a REST API with endpoints like:
           a)POST /students
           b)GET /students/{id}
           c)PUT /students/{id}
           e)DELETE /students/{id}
## 5)(Optional) Host Frontend
        i)Upload your HTML/JS frontend to an S3 bucket.
        ii)Enable static website hosting.

## 6)Test Your API
        i)Use Postman or curl to send requests and verify responses.

# SECURITY PERMISSIONS:
<>Ensure IAM roles are least-privilege.
<>Enable CORS on API Gateway if accessing from browser.
<>Set API keys or authentication if public access is not intended.


