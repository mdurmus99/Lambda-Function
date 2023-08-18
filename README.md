# AWS Lambda Snapshot Import Function
This AWS Lambda function is an instance that aims to take snapshots and manage EC2 instances with specific tags.

# How does it work?
This Lambda function scans EC2 instances with the labels "backup" or "Backup". It takes snapshots of the disks of the instances and stores them for the specified retention period. When the images expire, it automatically purges them.

# Installation and Use
Log in to the AWS Management Console.
Go to the Lambda service and create a new function.
Copy this code and edit your Lambda function.
Set the basic configuration of the Lambda function (for example, runtime and trigger).
Provide the necessary IAM permissions for the Lambda function to run.
Create an appropriate event trigger to trigger your Lambda function (for example, Amazon CloudWatch Events).
# Customization
You can customize this example function according to your needs:

**{'Name': 'tag-key', 'Values': ['backup', 'Backup']}** to specify different tags.
You can customize the retention time of snapshots with the Retention tag.

