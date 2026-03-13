# WordPress Dev/Test Environment Deployment - AWS

## Project Overview
Configured a WordPress instance for development and testing without affecting the live production environment.
The goal was to automate instance deployment, ensure controlled operational hours (9 AM to 6 PM), and optimize cost and governance using AWS services.

## Architecture Summary
- Isolated WordPress environment using CloudFormation
- Auto Scaling Group to manage instance count
- Lambda functions automate instance start/stop
- Route 53 monitors DNS for controlled availability
- CloudWatch used for logging and monitoring

## Technologies Used
- AWS EC2 & AMI
- CloudFormation
- Auto Scaling Group
- AWS Lambda
- EventBridge Scheduler
- Route 53
- WordPress CMS
- Apache / Nginx

## Deployment Process (AWS Console)
See `deployment-notes/cloudformation-deployment.md`

## Cost Optimization & Governance
- Scheduled instance start/stop prevents idle resource costs
- ASG scales dynamically during operational hours
- CloudFormation ensures repeatable, documented deployments

## Security Considerations
- IAM roles used for Lambda and EC2
- Security groups allow WordPress traffic only
- Instances isolated in dedicated VPC

## Result / Impact
- Created fully isolated dev/test environment
- Automations reduced operational cost
- Ensured live production environment remains unaffected
- Demonstrated AWS CloudFormation and Lambda orchestration skills

## Architecture Diagram
See `diagrams/wordpress-automation.svg`
