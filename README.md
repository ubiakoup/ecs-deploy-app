# ecs-deploy-app
The project aims to deploy a WordPress application in a serverless environment using AWS services. The application will be containerized and run using Amazon ECS (Elastic Container Service) and AWS Fargate for serverless management. AWS EFS (Elastic File System) will be integrated to ensure persistent and shared storage between the different WordPress instances.

The application needs to be highly available and secure, deployed across two availability zones to ensure resilience against single-zone failures. A Load Balancer will be implemented to handle traffic distribution between instances, and an Auto Scaling Group will ensure automatic scalability based on demand.

To enhance security, all traffic will be redirected from HTTP to HTTPS using Amazon Route 53 for DNS management, and AWS ACM (Certificate Manager) will be utilized for creating and managing SSL/TLS certificates.

For database management, Amazon RDS (Relational Database Service) will be used with a multi-AZ (Multi-Availability Zones) configuration, and an RDS Proxy will be implemented to optimize latency and manage database connections efficiently.

To monitor system performance and metrics, Amazon CloudWatch will be set up to collect and analyze logs and metrics, enabling proactive maintenance. AWS Secrets Manager will be used to securely manage secrets (such as database credentials), ensuring the safety of sensitive data.

This architecture ensures high availability, automatic scalability, and enhanced security for the WordPress application, with reliable data persistence and continuous performance monitoring.


![Architecture App](https://github.com/user-attachments/assets/8cc77043-fb4c-4cbc-903c-0a01eda9f4d0)
