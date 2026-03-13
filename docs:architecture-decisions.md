## Automation & IaC
- AWS CloudFormation chosen to provision repeatable infrastructure
- Lambda used for automatic instance management during off-hours

## Auto Scaling
- ASG ensures correct instance count during business hours
- Prevents over-provisioning

## DNS & Monitoring
- Route 53 monitors availability and health
- CloudWatch used for logging and alerts

## Security
- Security Groups restrict HTTP/HTTPS
- IAM roles replace credentials in scripts

## Cost Optimization
- Off-hours instance stop via EventBridge reduces costs
- ASG only scales during defined hours}
