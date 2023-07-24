# Building Serverless Architecture Using AWS
The project aims to build a serverless architecture on AWS, leveraging various services to create an efficient and scalable system for handling CRUD operations (Create, Read, Update, Delete) through HTTP APIs. The key resources involved in this architecture are Amazon API Gateway, Lambda functions, and DynamoDB.

<h3>1. Amazon API Gateway:</h3>
Amazon API Gateway acts as the entry point for all incoming HTTP requests. It allows the creation of HTTP APIs with different endpoints, each backed by a separate Lambda function. This enables the system to have a clear and structured API design, making it easier to manage and scale as the project grows.

<h3>2. Lambda Functions for CRUD Actions:</h3>
For each endpoint defined in the API Gateway, a corresponding Lambda function is implemented to handle the respective CRUD operation. Lambda functions are serverless compute resources that can be automatically scaled based on demand, allowing the system to efficiently handle varying levels of incoming traffic. These functions act as the core business logic, processing requests, and interacting with the data stored in DynamoDB.

<h3>3. DynamoDB Table:</h3>
DynamoDB is a fully managed, serverless NoSQL database service provided by AWS. In this project, a DynamoDB table is created to store the data required for the CRUD operations. DynamoDB offers seamless scalability and high availability, ensuring the application can handle large volumes of data and requests without downtime.

<h3>4. Provisioning Environment and User Permissions:</h3>
To deploy the serverless architecture successfully, the project includes provisioning the necessary environment, including the Lambda functions, API Gateway, and DynamoDB table. Additionally, the appropriate IAM (Identity and Access Management) roles and permissions are set up to ensure secure access to resources and protect against unauthorized access.

<h3>5. Lambda Layers using PynamoDB:</h3>
Lambda Layers are used to share common code across multiple Lambda functions. This project uses Lambda Layers to integrate PynamoDB, an object relationship mapper for DynamoDB. PynamoDB simplifies communication with DynamoDB by abstracting away low-level details and providing a more convenient way to interact with the database. This promotes code reusability and ensures consistent interactions with the data stored throughout the Lambda functions.
<br><br>

<h2>Architecture:</h2>
This serverless architecture contains HTTP APIs where every single endpoint is backed by a separate lambda function. These lambda functions communicate with DynamoDB database, which is a serverless NoSQL database. Finally, the lambda layers are used to share codes using PynamoDB, an object relationship mapper, which is a convenient way to communicate with DynamoDB. 
We perform the following tasks in order to deploy this architecture:

* Create Lamda function for CRUD (Create, Read, Update, Delete) actions.
* Create Amazon API gateway HTTP API.
* Create DynamoDB table.
* Provision the environment and user permissions.
* Create lambda layers using PynamoDB.

The project's serverless architecture provides a cost-effective, highly available, and scalable solution for handling CRUD operations through HTTP APIs. It efficiently manages resources, reduces the need for server maintenance, and simplifies the database interactions using PynamoDB through Lambda Layers.
<br>

<img width="468" alt="image" src="https://github.com/anshi1995/Building-Serverless-Architecture-Using-AWS/assets/101793943/68d001be-b6c2-49c5-aa9c-7be5234b5b39">
