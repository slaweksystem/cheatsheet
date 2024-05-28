# EC2

This file is dedicated for EC2 Instance.

Amazon EC2 - Virtual Servers in the Cloud

- Limited by RAM and CPU
- Continously running
- Scaling means intervention to add/remove servers

## EC2 Instance Launch Types

- On Demand Instances: short workload, predictable pricing
- Reserved Instances: long workloads (>= 1 year)
  - Convertible Reserved Instances: long workloads with flexible instances
  - Scheduled Reserved Instances: launch within time window you reserve
- Spot Instances: short workloads, for cheap, can lose instances
- Dedicated Instances: no other customers will share your hardware
- Dedicated Hosts: book an entire physical server, control instance placement

### EC2 On Demand

- Pay for what you use (billing per second, after the first minute)
- Has the highest cost but no upfront payment
- No long term commitment

Usecase:

- Recommended for short-term and un-interrupted workloads, where you can't predict how the application will behave.

### EC2 Reserved Instance

- Up to 75% discount compared to On-demand
- Pay upfront for what you use with longterm commitment
- Reservation period can be 1 to 3 years
- Reserve a specific instance type
- Recommended for steady state usage applications (think database)

- __Convertible Reserved Instance:__
  - can change the EC2 instance type
  - up to 54% discount
- __Scheduled Reserved Instances__
  - launch within time window you reserve
  - When you require a fraction of day/week/month

### EC2 Spot Insances

- Can get a discount of up to 90% compared to On-demand
- You bid a price and get the instance as long as its under the price
- Price will varie based on offer and demand
- Spot instances are reclaimed with a 2 minute notification watrning when the spot price goes above your bid

Usecase:

- Used for batch jobs, Big Data analysis, or workloads that are resilient to failures.

### EC2 Dedicated Hosts

- Physical dedicated EC2 server for your use
- full control of EC2 Instance placement
- Visibility into underlying sockets / physical cores of the hardware
- Allocated for your account for a 3 year period reservation
- More expensive

Usecase:

- Useful for software that have complicated licensing model (BYOL - Bring Your Own License)
- For companies that have strong regulatory or compliance needs

### EC2 Dedicated Instances

- Instances running on hardware that's dedicated to you
- May share hardware with other instances in same account
- No control over instance placement (can move hardware after Stop/Start)

### Which host is right for me

![AWS-EC2-Right-For-Me](img/AWS-EC2-Right-For-Me.png)

## Shutdown Behaviour

- __Shutdown behaviour:__ How should the instance react when shutdown is done using the OS?
  - Stopped: default
  - Terminated

- This is not applicable from AWS console or AWS API.
- CLI Attribute: `InstanceInitiatedShutdownBehavior`

### Termination Protection

- Enable termination protection: to protect against accidental termination in AWS Console or CLI

- __Exam Tip:__
  - We have an instance where shutdown behavior = terminate and enable terminate protection is ticked
  - We shutdown the instance from the OS, what will happen?
    - The instance will still be terminated.

### Placement Groups

Sometimes you want to control over EC2 Instance placement strategy.  
That strategy can be defines using placemnet groups.  
When you create a placement group, you specify one of the following strategied for the group:

- Cluster -- clusters instances into low-latency group in a ssingle Availability Zone.
- Spread -- spreads instances across underlying hardware(max 7 instances per group per AZ) - critical applications
- Partition -- spreads instances across many different partitions (which rely on different sets of racks) within an AZ. Scales to 100s of EC2 instances per group (Hadoop, Cassandra, Kaftka).

#### Placement Groups - Cluster

![AWS-Placement-Groups-Cluster](img/AWS-Placement-Groups-Cluster.png)

#### Placement Groups - Spread

![AWS-Placement-Groups-Spread](img/AWS-Placement-Groups-Spread.png)

#### Placement Groups - Partition

- Partitions are different set of racks

![AWS-Placement-Groups-Partition](img/AWS-Placement-Groups-Partition.png)

## Cloudwatch Metrics for EC2

- AWS Procided metrics (AWS pushes them):
  - Basic Monitoring (default): metrics are collected a 5 minute interval
  - Detailed Monitoring (paid): metrics are collected at 1 minute interval
  - Includes CPU, Network, Disk and Status check Metrics

- Custom metric (yours to push):
  - Basic Resolution: 1 minute resolution
  - High resolution: all the way to 1 second resolution
  - Include RAM, application level metrics
  - Make sure the IAM permissions on the EC2 instance role are correct!

### EC2 included metrics

- __CPU:__ CPU Utilization + Credit Usage / Balance
- __Network:__ Network In/Out
- __Status Check:__
  - Instance status = check the EC2VM
  - System status = check the underlying hardware
- __Disk:__ Read/Write for Ops/Bytes (only for instance store)

__Note:__ _Ram is not included in the AWS metrics_


