# AWS CloudFormation

CloudFormation is a declaritive way of outlining your AWS Infrastructure, for any resources (most of them are supported).

For example, within a CloudFormation template, you say:

- I want a security group
- I want two EC2 machines using this security group
- I want two Elastic IPs for these EC2 machines
- I want an S3 bucket
- I want a load balancer (ELB) in front of these machines

The CloudFormation creates those for you, in the __right order__, with the __exact configuration__ that you specify.

The whole definition of your whole architecure is in one file. That file is declaritive.
