# ServerlessWebApplication
<h2>Description:</h2>
This project is a web application that is built using serverless architecture on the Amazon Web Services (AWS) platform. The goal of this project is to leverage AWS services to create a scalable, cost-effective, and highly available web application without the need for managing traditional servers.
<h2> Key Components and Services used:</h2>

1. AWS Lambda: AWS Lambda is used to run the application's backend code in a serverless manner. It allows you to execute code in response to events, such as HTTP requests or database updates.

2. Amazon API Gateway: API Gateway is used to create RESTful APIs that act as the entry point for the web application. It handles requests from clients and routes them to the appropriate Lambda functions.

3. Amazon S3: S3 (Simple Storage Service) is used to store static assets of the web application, such as HTML, CSS, JavaScript files, and images.

4. Amazon DynamoDB: DynamoDB is a NoSQL database service provided by AWS. It is used to store and retrieve data for the web application. DynamoDB offers scalability, low latency, and automatic scaling.

5. Amazon Cognito: Cognito is used for user authentication and authorization. It provides a secure way to manage user sign-up, sign-in, and access control for the web application.

6. AWS CloudFormation: CloudFormation is used for infrastructure as code. It allows you to define and provision AWS resources in a declarative manner, making it easier to manage and deploy the application infrastructure.

7. AWS CloudFront: CloudFront is a content delivery network (CDN) service provided by AWS. It is used to distribute the web application's static assets globally, reducing latency and improving performance.

8. AWS Route 53: Route 53 is a scalable and highly available domain name system (DNS) service provided by AWS. It is used to route incoming requests to the web application's API Gateway and CloudFront distribution.
<h2>Project Workflow:</h2>

1. Design the architecture: Define the components and services required for the web application, including API Gateway, Lambda functions, DynamoDB tables, S3 buckets, and IAM.
<p align="center">
Serverless Architecture: <br/>
<p align="center">
<img src="https://imgur.com/Je2E7Ju.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/R4cMuGd.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/qebd2lc.png" height="80%" width="80%">
<br />

2. To host our Website, we will choose Amplify. With Amplify, we can build and host websites. For our purpose, since our website is very simple we will create an html file in a text editor on our local machine and just use Amplify to deploy and host that webpage. The code for this is given above in the INDEX.HTML ORIGINAL file. Just copy and Paste this code in your file. Once you have created this file, Zip it by just right clicking on the file and selecting compress. 
<p align="center">
<img src="https://imgur.com/aVIMe8P.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/He6z40O.png" height="80%" width="80%">
<br />

3. On the AWS Console, navigate to AWS Amplify and click on New App. Here, just click on Deploy Without Git Provider, Enter a name for the App and Environment name and Choose and upload the Zip file.
<p align="center">
<img src="https://imgur.com/XqZrgem.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/4GSgo4a.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/ZBPB2LS.png" height="80%" width="80%">
<br />

4. From AWS Console, navigate to AWS Lamda. Click on New function. Enter the details, scroll down to the code blovk









5. Develop Lambda functions: Write the backend code for the web application's functionality using programming languages supported by Lambda, such as Node.js, Python, or Java.

6. Create API Gateway: Configure API Gateway to define the RESTful APIs and integrate them with the appropriate Lambda functions.

7. Set up DynamoDB: Create the necessary DynamoDB tables to store and retrieve data for the web application.

8. Implement user authentication: Configure Cognito user pools to handle user sign-up, sign-in, and access control for the web application.

9. Store static assets: Upload the web application's static assets, such as HTML, CSS, JavaScript files, and images, to S3 buckets.

10. Configure CloudFront: Set up CloudFront to distribute the static assets globally and improve performance.

11. Deploy the application: Use CloudFormation to define the infrastructure as code and provision the required AWS resources.

12. Test and monitor: Test the web application's functionality and performance. Set up monitoring and logging using AWS CloudWatch to track and analyze application metrics.
<h2>Benefits of AWS WordPress Website:</h2>

1. Scalability: The serverless architecture allows the web application to scale automatically based on demand, ensuring optimal performance even during high traffic periods.

2. Cost-effectiveness: With serverless, you only pay for the actual usage of resources, eliminating the need for provisioning and managing servers, which can result in cost savings.

3. High availability: AWS services, such as Lambda and DynamoDB, are designed to be highly available and fault-tolerant, ensuring the web application remains accessible even in the event of failures.

4. Reduced operational overhead: Serverless architecture offloads the operational tasks, such as server management, to AWS, allowing developers to focus more on application development and business logic.
<br/>
