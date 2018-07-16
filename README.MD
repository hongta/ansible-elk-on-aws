# Ansible for ELK on AWS

## Setup

### EC2 for Ansible instance
Setup and install Ansible on the EC2 instance, and allow this instance to create AWS resources.
#### Assign the role to the instance
#### Install Python3, PIP3 and Ansible
```
> sudo yum install python3

> python3 --version
Python 3.7.0rc1 (default, Jun 20 2018, 02:13:35)
[GCC 7.3.1 20180303 (Red Hat 7.3.1-5)]

> pip3 --version
pip 9.0.3 from /usr/lib/python3.7/site-packages (python 3.7)

> pip3 install ansible  --user
...
> which ansible
~/.local/bin/ansible

## Usage

### Parameters required
 - `vpc_id` for security group
 - `subnets` for application Load balancer

## Roles
### Logstash

- EC2 instances
- Application LoadBalancer
- Security Group for ALB