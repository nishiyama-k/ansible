## Overview

Construct autoscaling sample environment on AWS

## Prerequisites

- python 3.5.2
- ansible 2.9.9
- boto3 1.14.1
- awscli 1.18.5

## Architecture

- VPC
- Multi AZ
- Public / Private Subnet
- Nat Gateway
- Bastion Server
- Web Server
- AP Server
- DB Server
- Spot Instance
- S3
- WAF

# How to Use
## IAM User
- EC2 Access
- VPC Access
- CloudFormation Access
- WAF Access
- S3 Access

## Construct
```
ansible-playbook construct-on-aws.yml --extra-vars="AWS_ACCESS_KEY_ID='xxxx' AWS_SECRET_ACCESS_KEY='xxxx' AWS_REGION='ap-northeast-1'"
```
## Terminate
```
ansible-playbook terminate-on-aws.yml --extra-vars="AWS_ACCESS_KEY_ID='xxxx' AWS_SECRET_ACCESS_KEY='xxxx' AWS_REGION='ap-northeast-1'"
```