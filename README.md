# Cloud Computing Project – Scalable AWS Architecture for Web Application

## Project Overview

This project demonstrates the migration of a LAMP stack web application from a local desktop environment to a cloud-based architecture using Amazon Web Services (AWS). The architecture is designed for a small startup anticipating rapid and unpredictable growth. The key focus areas are scalability, availability, disaster recovery, and cost-efficiency.

This project was developed as part of the final assessment for the subject "Cloud Computing and Software as a Service (41001)" and contributes 35% toward the final grade.

## Objectives

- Design a scalable, highly available, and fault-tolerant cloud architecture.
- Implement elastic infrastructure capable of adapting to changing load conditions.
- Apply AWS best practices for disaster recovery and performance.
- Justify service selection with respect to business requirements.

## Deliverables

### Deliverable 1 – Architecture Documentation
- System architecture diagram.
- Service justification and architectural assumptions.
- List of AWS services and their configurations.

### Deliverable 2 – AWS Deployment
A complete AWS environment built using either:
- AWS Elastic Beanstalk, or
- Individually configured AWS services.

## AWS Services Used

- Amazon EC2 with a custom AMI
- Elastic Load Balancer (ELB)
- Auto Scaling Group (min 2, max 8 instances)
- Amazon RDS with Multi-AZ deployment (MySQL)
- Elastic Beanstalk (optional orchestration)
- Custom Security Group (allowing HTTP and SSH)
- Custom Virtual Private Cloud (VPC) with two public subnets in separate Availability Zones
- Custom Key Pair for SSH access
- Email notifications for environment changes

## Scaling Configuration

- Auto scaling based on EC2 network output traffic
  - Upper threshold: 60%
  - Lower threshold: 30%


## References

- AWS Elastic Beanstalk Documentation  
  https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/GettingStarted.html
- RDS Web App Deployment  
  https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_Tutorials.WebServerDB.CreateWebServer.html
- Auto Scaling and Load Balancing  
  https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-register-lbs-with-asg.html
- LAMP Stack on EC2  
  https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/install-LAMP.html
