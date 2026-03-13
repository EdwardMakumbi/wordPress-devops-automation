# Deployment Notes for WordPress Dev/Test

### Step 1: CloudFormation Stack
1. Create a new CloudFormation stack.
2. Define VPC, subnets, EC2 instances, security groups, and IAM roles.
3. Configure AMI for WordPress instance.
4. Deploy stack.

### Step 2: Auto Scaling Group
1. Create ASG linked to WordPress AMI.
2. Set min/max instance counts.
3. Assign target group for load balancing if needed.

### Step 3: Scheduled Automation
1. Create Lambda functions to start/stop instances.
2. Configure EventBridge schedule (9 AM to 6 PM).
3. Test automation triggers.

### Step 4: Monitoring
1. Configure CloudWatch metrics for EC2 and ASG health.
2. Set alerts for instance failure or scaling events.

### Step 5: DNS
1. Use Route 53 for domain access.
2. Verify availability and functionality.
