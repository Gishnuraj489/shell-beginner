# AWS Resource Lister 🛠️

A simple Bash script to list various AWS resources based on region and service using the AWS CLI.

## 📌 Description

This script allows you to quickly list AWS resources like EC2 instances, S3 buckets, RDS databases, and more by specifying the AWS region and service. It is useful for DevOps engineers, cloud administrators, and learners who want a fast way to inspect AWS resources from the command line.

## ✅ Prerequisites

- **AWS CLI** must be installed and configured.
- AWS credentials and permissions to access listed services.
- Bash environment (Linux/Mac or WSL/MinGW on Windows).

## 🔧 Installation

1. Clone the repository or copy the script to your local machine:
   ```bash
   git clone https://github.com/<your-username>/aws-resource-lister.git
   cd aws-resource-lister
Make the script executable:

bash
Copy
Edit
chmod +x aws_resource_list.sh
🚀 Usage
bash
Copy
Edit
./aws_resource_list.sh <aws_region> <aws_service>
🧾 Example
bash
Copy
Edit
./aws_resource_list.sh us-east-1 ec2
💡 Supported AWS Services
Service	Keyword
EC2 Instances	ec2
RDS Instances	rds
S3 Buckets	s3
CloudFront	cloudfront
VPCs	vpc
IAM Users	iam
Route 53	route5*
CloudWatch	cloudwatch
CloudFormation	cloudformation
Lambda	lambda
SNS Topics	sns
SQS Queues	sqs
DynamoDB	dynamodb
EBS Volumes	ebs

⚠️ Note: Route 53 is listed as route5 in the script. You may want to correct this to route53 for consistency.

📂 Output
Each command displays the AWS CLI JSON output of the selected service's resources.

🛡️ Error Handling
Validates if AWS CLI is installed and configured.

Checks for correct number of arguments.

Handles invalid service input gracefully.

📄 License
This project is licensed under the MIT License.

🤝 Contributions
Feel free to fork, improve, and submit a pull request! Suggestions are always welcome.
