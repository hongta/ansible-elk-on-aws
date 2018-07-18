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

> pip install ansible boto3 --user
...
> which ansible
~/.local/bin/ansible
```

## Usage

### Parameters required
 - `vpc_id` for security group
 - `subnets` for application Load balancer

## Roles

### java
Install java 1.8 for Logstash and Elasticsearch

### AWS-Logstash
tasks to setup AWS infra and Logstash servers

- Security Group for EC2 instance
- EC2 instances
- Target Group
- Application LoadBalancer

### Service-Logstash
Install Logstash and configuraiton



### AWS-Elasticsearch
tasks to setup AWS infra for Elasticsearch servers

- Security Group for EC2 instances
- EC2 instances

### Elastic.Elasticsearch
Official Elasticsearch playbook

## Referrers
 - [ansible-logstash](https://github.com/wunzeco/ansible-logstash/blob/master/handlers/main.yml)