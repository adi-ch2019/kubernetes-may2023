# Cloud clusters minimal setups
## AWS EKS
- Core concepts to be aware about are
  - [Amazon EKS (Elastic Kubernetes Service)](https://docs.aws.amazon.com/cli/latest/reference/eks/index.html)
  - [Amazon Elastic Compute Cloud (EC2) - CLI reference docs for this](https://docs.aws.amazon.com/cli/latest/reference/ec2/)
  - [Amazon Virtual Private Cloud (VPC)](https://docs.aws.amazon.com/vpc/latest/mirroring/what-is-traffic-mirroring.html)
  - [AWS Identity and Access Management (IAM)](https://docs.aws.amazon.com/rolesanywhere/latest/userguide/introduction.html)

To get started with Amazon EKS ,you need to create an Amazon EKS cluster and then launch worker nodes into your cluster. You can do this using the AWS Management Console, AWS CLI, or programmatically using AWS SDKs or Infrastructure as Code (IaC) tools like Terraform and CloudFormation. Once your cluster is up and running, you can use standard Kubernetes tools and APIs to deploy and manage your applications. 

EC2 offers users persistent storage and elastic IP addresses while being fault-tolerant thanks to Amazon's engineering of Availability Zones insulated from other availability zones. There are multiple ways to pay for EC2 instances such as On-Demand, Savings Plans, Reserved Instances, and Spot Instances based on each use-case and budget.

VPC service provides users with the option to assign IP addresses of their choosing from one or more subnets, giving them granular control over security by choosing which AWS resources are public facing or not. VPC allows users to connect to the internet, a user's corporate data center, and other users' VPCs. The security of AWS VPC is ensured through the use of security groups as a firewall to control traffic at the instance level, and network access control lists as a firewall to control traffic at the subnet level.

With IAM, you can create and manage AWS users and groups, set permissions for resources, control access to AWS services, and manage multiple users and their level of access to AWS resources from a single AWS account. IAM provides various features, such as multi-factor authentication, password policies, and permissions boundaries, to help you manage access securely. 

## Prerequisites for AWS EKS on your Linux PC or Server include
- kubectl
- AWS CLI
- eksctl
- AWS Free Account
