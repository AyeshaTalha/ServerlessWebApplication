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

4. We need to create a Lamda Function that will process our math functionality. From AWS Console, navigate to AWS Lamda. Click on New function. We are going to author this from scratch. Enter thr name of thr Function, Runtime as the latest version of Python and click on Create Function.On the main page of Lamda, scroll down to the Code block. The code for this Lamda Function is given in the LamdaFunctionOriginal file above. Just copy and paste the code. Click on Deploy and we are done.
<p align="center">
<img src="https://imgur.com/XnvzGhE.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/b8ejCFq.png" height="80%" width="80%">
<br />

5. Now, we need something to invoke our Math Functionality. For this, we will use API Gateway. This is a core functionality in AWS which we can use to create our own APIs. In a Serverless Architrcture, it is the perfect way to invoke our Lamda Function. From the AWS Console, navigate to API Gateway and Click on Create API. We are going to use a REST API. Give it a name and click on Create API. 
<p align="center">
<img src="https://imgur.com/vCsjcMa.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/2U90adI.png" height="80%" width="80%">
<br />

6. Click on the API created. On the lefthand side, click on Resources. On the righthand side, click on "/". From thr Actions menu, select Create Method. The type of method will be POST. Enter the Lamda Function name and create the POST method as shown below:
<p align="center">
<img src="https://imgur.com/YTPA3rb.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/8a0masw.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/srGDfkU.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/srGDfkU.png" height="80%" width="80%">
<br />

7. Next, we must Enable CORS (Cross Origin Resourse Sharing) so that our website can interact with the lamda function. To do so, click on the POST method and from Actions menu select Enable CORS. Click on Deploy API to deploy and enter the Deployment stage as dev.
<p align="center">
<img src="https://imgur.com/SItVLAs.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/jXU9YV6.png" height="80%" width="80%">
<br />
<p align="center">
<img src="https://imgur.com/izfqvWx.png" height="80%" width="80%">
<br />













6. Develop Lambda functions: Write the backend code for the web application's functionality using programming languages supported by Lambda, such as Node.js, Python, or Java.

7. Create API Gateway: Configure API Gateway to define the RESTful APIs and integrate them with the appropriate Lambda functions.

8. Set up DynamoDB: Create the necessary DynamoDB tables to store and retrieve data for the web application.

9. Implement user authentication: Configure Cognito user pools to handle user sign-up, sign-in, and access control for the web application.

10. Store static assets: Upload the web application's static assets, such as HTML, CSS, JavaScript files, and images, to S3 buckets.

11. Configure CloudFront: Set up CloudFront to distribute the static assets globally and improve performance.

12. Deploy the application: Use CloudFormation to define the infrastructure as code and provision the required AWS resources.

13. Test and monitor: Test the web application's functionality and performance. Set up monitoring and logging using AWS CloudWatch to track and analyze application metrics.
<h2>Benefits of AWS WordPress Website:</h2>

1. Scalability: The serverless architecture allows the web application to scale automatically based on demand, ensuring optimal performance even during high traffic periods.

2. Cost-effectiveness: With serverless, you only pay for the actual usage of resources, eliminating the need for provisioning and managing servers, which can result in cost savings.

3. High availability: AWS services, such as Lambda and DynamoDB, are designed to be highly available and fault-tolerant, ensuring the web application remains accessible even in the event of failures.

4. Reduced operational overhead: Serverless architecture offloads the operational tasks, such as server management, to AWS, allowing developers to focus more on application development and business logic.
<br/>
