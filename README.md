cloudformation.subnet
=====================


## Description:

This CloudFormation stack creates a subnet within [AWS VPC](https://aws.amazon.com/vpc/).

## Prerequisites:

* An AWS account and environment configured with appropriate AWS Credentials.
* A VPC should be created beforehand.

## See how it works:

AWS Management Console

* Login to AWS Management Console
* Launch in CloudFormation the subnet.yaml stack (from the repo you cloned), provide required parameters.


Stack Parameters
----------------
| Name                 | Description                 | Default value    |
|:---------------------|:----------------------------|:-----------------|
| VPC                  | A VPC Id                    | [Mandatory]      |
| AvailabilityZone     | An AvailabilityZone         | [Mandatory]      |
| InternetGateway      | An InternetGateway Id       | [Optional]       |
| CidrBlock            | A subnet CIDR block         | `10.0.0.0/24`    |
| Type                 | A subnet type               | `private`        |
| Name                 | A subnet name               | "${Type}-subnet" |


Stack Outputs
-------------
| Name           | Description                  |
|:---------------|:-----------------------------|
| SubnetId       | A subnet Id                  |


# Author
Dmitrii Ageev <d.ageev@gmail.com>

