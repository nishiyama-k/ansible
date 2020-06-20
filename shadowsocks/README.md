## Overview

Construct Shadowsocks server on AWS

## Prerequisites

- python 3.5.2
- ansible 2.9.9
- boto3 1.14.1
- awscli 1.18.5

## Architecture

- VPC
- An AZ
- A Subnet
- An EC2Instance where shadowsocks is installed

# How to Use
## IAM User
- EC2 Access
- VPC Access

## Construct
```
ansible-playbook construct-shadowsocks-on-aws.yml --extra-vars="AWS_ACCESS_KEY_ID='xxxx' AWS_SECRET_ACCESS_KEY='xxxx' AWS_REGION='ap-northeast-1'"
```
## Terminate
```
ansible-playbook terminate-shadowsocks-on-aws.yml --extra-vars="AWS_ACCESS_KEY_ID='xxxx' AWS_SECRET_ACCESS_KEY='xxxx' AWS_REGION='ap-northeast-1'"
```