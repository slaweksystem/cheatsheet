# AWS-AMI

## What's an AMI?

As we saw, AWS comes with base images such as:

- Ubuntu
- Fedora
- RedHat
- Windows Etc...

These images can be customised at runtime using EC2 User data

But what if we could create our own image, ready to go?

That's an AMI - an image to use to create our instances

AMIs can be built for Linux or Windows machines

## Why would you use a custom AMI?

- Using a custom build AMI can provide the following advantages:
  - Pre-installed packages needed
  - Faster boot time (no need for long ec2 user data at boot time)
  - Machine comes configured with monitoring/enterprise software
  - Security concerns - control over the machines in the network
  - Control of maintenance and updates of AMI's over time
  - Active Directory Integration out of the box
  - Installing your app ahead of time (for faster deploys when auto-scaling)
  - Using someone else's AMI that is optimised for running an app, DB, etc...
- __AMI are build for a specific AWS region (!)__
