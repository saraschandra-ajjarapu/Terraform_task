# terraform_task

   ELTROPY DEVOPS ASSIGNMENT

DevOps assignment
Instructions
1.	This is an assignment to test your skills to setup server infrastructure on AWS cloud
2.	You may do research and implement the best practices
3.	Use your personal AWS account to configure this
Detailed Assignment 
1.	Create a VPC
2.	Create EC2 instance using Ubuntu Linux 
3.	Enable and configure Security Group
4.	Server Hardening
1.	Research and execute server hardening on this instance 
2.	For example (but not limited to the following, implement more if possible)
1.	SSH on non-standard port
2.	Disabled Password based Sign in
3.	Configure UFW (Ubuntu Firewall)
4.	Disable root access
5.	VPN - Enable Access only through OpenVPN to this instance
6.	CloudWatch - Setup CloudWatch for Disk size and CPU
1.	Enable Email alerts for alerts
7.	Enable ClamAV - Free Antivirus for Linux
8.	Backup
1.	Enable backup for instances
Architecture: 


AWS Services:  VPC, EC2, S3, CloudWatch, SNS, SQS, NAT gateway
Tools & Technologies : Terraform version : 13, Ansible version: 2.9, Shell script, AWS CLI
Development/Enhancements :

•	Having AWS managed IAM policies (Ex:Instance-profiles, roles),
•	Using AWS SSM to manage infrastructure within AWS,
•	Packer for Golden Image Creation and Terraform for Infra and Dynamic host/server configuration with Ansible.
•	Cross Region VPC peering.
•	CloudWatch Data source Integration with Prometheus/Grafana Dashboards.
•	Envoy Proxy to route part of traffic to QA testing.

Create VPC:
                     
                     
                       
 
 
•	I have used terraform for infrastructure setup which creates VPC, Private and Public subnets, internet gateway, NAT gateway, route tables, EC2 instances and security groups.
Create EC2 instance using Ubuntu Linux:
 
                 
             
Enable and configure Security Group:
 
Server Hardening
•	I have used ansible as a configuration management tool.
•	I have used UFW module, Shell module, handlers and few configurations to setup the server.
•	SSH on non-standard port
•	Disabled Password based Sign in
•	Configure UFW (Ubuntu Firewall)
•	Disable root access
 
 



OpenVPN:
 

CloudWatch:
 
 
 




Enable ClamAV:
 
EC2 Instance Backup: 
 
 





