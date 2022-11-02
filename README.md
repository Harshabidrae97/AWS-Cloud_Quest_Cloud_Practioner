## AWS-Quest-Cloud-Practitioner : Solutions Built

Highly Available Web Applications
- Help the travel agency create a highly available web application.
- Created an Application Load Balancer(ALB)
- Configure an Auto Scaling Group and connect it to the ALB.
- Configured a health check endpoint.
- Configured an Auto Scaling Group to include a new EC2 instances in multiple Availability Zones (Az).
![Screen Shot 2022-09-11 at 3 11 57 PM](https://user-images.githubusercontent.com/55474202/189547060-f0c174eb-9fe4-4b40-9aa0-743fd7a6d7f7.png)

## AWS Cloud Economics.
- created an estimation of architecture using the AWS Pricing Calculator.
- Change the EC2 instance type to t2.micro and generated new price estimate URL.![Screen Shot 2022-09-11 at 3 23 15 PM](https://user-images.githubusercontent.com/55474202/189547450-f5018967-5f43-462f-9b49-86c85406ba2f.png)

## Auto healing and Scaling Applications.
- Created an EC2 template from an existing EC2 instance.
- Configured an Auto Scaling Group with minimum of two and maximum of 4 instances.
- Assigned a CPU utilization metric and schedule based on Auto Scaling rules.
- Configured an Auto Scaling policy to scale down to 0 resources at 1 AM UTC every day.![Screen Shot 2022-09-11 at 3 30 03 PM](https://user-images.githubusercontent.com/55474202/189547677-8a2b2048-445d-4117-89b7-226b57458b97.png)

## Core Security Concepts.
- Helps to improve security at the city's stock exchange by ensuring that support engineers can only perform authorized actions.
- Created a SupportEngineers group.
- Attached a policy that allows group members to read only access to EC2.
- Verified that group members have read only EC2 Access.
- Granted the support Engineers group read only access to RDS.![Screen Shot 2022-09-11 at 3 36 13 PM](https://user-images.githubusercontent.com/55474202/189547891-51160940-e4ce-4899-ad72-550b7f423107.png)

## Networking Concepts.
- Helps the bank setup a seccure networking environment which allows communications between resources and the inernet.
- Changed the WebServer subnet from private to public.![Screen Shot 2022-09-11 at 3 41 48 PM](https://user-images.githubusercontent.com/55474202/189548080-ab5c6e8a-d76b-4d4a-83f8-465b60351f63.png)

- Configured a security group to allow HTTP traffic from the internet.
- Configured the Security group rules to allow traffic over port 3306 into DataBase Server. 

## Migration Concepts.
- https://d2908q01vomqb2.cloudfront.net/77de68daecd823babbb58edb1c8e14d7106e83bb/2019/05/21/Tech-Mahindra-Telia-1.png![image](https://user-images.githubusercontent.com/55474202/199589311-387a753f-6937-46ee-ac2e-6835b4db9177.png)

-
Tech Mahindra-Telia-1

- The following AWS services and features now host components of Telia’s new CIM microservice architecture:

- AWS VPN establishes a secure and private tunnel from the on-premises data center to the AWS global network.
- Amazon Route 53 is a Domain Name Server (DNS), which routes global traffic to the application using Elastic Load Balancing.
- Amazon Virtual Private Cloud (Amazon VPC) sets up a logically isolated, virtual network where the application can run securely.
- Application Load Balancer is a product of Elastic Load Balancing, which load balances HTTP/HTTPS applications and uses layer 7-specific features, like     port and URL prefix routing for containerized applications.
- Amazon Elastic Container Service (Amazon ECS) is a container orchestration service that supports Docker containers to run and scale containerized           applications on AWS.
- AWS Fargate is a compute engine for Amazon ECS that allows running containers without having to manage servers or clusters. Microservices are deployed as   Docker containers in the Fargate serverless model.
- Amazon Elastic Container Registry (ECR) is integrated with Amazon ECS as a fully managed Docker container registry that makes it easy to store, manage,     and deploy Docker container images. This is used as a private repository to host built-in Docker images.
- Amazon Aurora is a relational database compatible with MySQL and PostgreSQL, used as a database for the CIM platform migration.
- AWS DMS migrates on-premises Oracle databases to cloud-native Aurora databases.
- Amazon CloudWatch is a monitoring and management service used to monitor the entire CIM platform and store application logs for analysis.
- Amazon Elastic Compute Cloud (Amazon EC2) provides compute capacity in the cloud, and was used to host Jenkins and JFrog Artifactory as a container for     the CI/CD pipeline.
- AWS Identity and Access Management (IAM) manages access to AWS services and resources securely.
