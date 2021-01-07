# quickstart-uipath-robot
## UIPath Robot on AWS Cloud

This Quick Start reference deployment guide provides step-by-step instructions for deploying UiPath Robot on AWS Cloud.

This Quick Start is for users who wants to deploy UiPath Robot application on AWS cloud. It deploys UiPath Robot which helps with robotic automation processes, allowing users to automate attended and unattended process task within their enterprise environment. 

The AWS CloudFormation templates included with the Quick Start automate the following:

- [Deploying the UiPath Robot on AWS Cloud](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/template?stackName=uipath&templateURL=https://aws-quickstart.s3.amazonaws.com/quickstart-uipath-robot/templates/main.template.yaml)

You can also use the AWS CloudFormation templates as a starting point for your own implementation.

![Quick Start architecture for UiPath Robot on AWS](./UiPath-Robot-arch.png)

As shown in the architecture for UiPath Robot, the Quick Start sets up the following:

* A highly available architecture that spans two (or more) Availability Zones, per your choosing.
* A VPC configured with public and private subnets, according to AWS best practices, to provide you with your own virtual network on AWS.*

In the public subnets:
* Managed network address translation (NAT) gateways to allow outbound internet access for resources in the private subnets.*
* A Windows bastion host to allow inbound RDP access to EC2 instances in private subnets.

In the private subnets:
* The EC2 machines hosting UiPath Robot

_You are responsible for the cost of the AWS services used while running this Quick Start. There is no additional cost for using the Quick Start._