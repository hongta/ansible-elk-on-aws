# Ansible for ELK on AWS

## Setup

### EC2 for Ansible instance
Setup and install Ansible on the EC2 instance, and allow this instance to create AWS resources.
#### Assign the role to the instance
#### Install Python, PIP and Ansible
```
> sudo yum install python

> python --version
Python 2.7.14

> pip --version
pip 9.0.3 from /usr/lib/python2.7/site-packages (python 2.7)

> pip install ansible  --user
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