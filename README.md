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

## Notices
This document is provided for informational purposes only. It represents AWS’s current product offerings and practices as of the date of issue of this document, which are subject to change without notice. Customers are responsible for making their own independent assessment of the information in this document and any use of AWS’s products or services, each of which is provided “as is” without warranty of any kind, whether expressed or implied. This document does not create any warranties, representations, contractual commitments, conditions, or assurances from AWS, its affiliates, suppliers, or licensors. The responsibilities and liabilities of AWS to its customers are controlled by AWS agreements, and this document is not part of, nor does it modify, any agreement between AWS and its customers.

The software included with this paper is licensed under the Apache License, version 2.0 (the "License"). You may not use this file except in compliance with the License. A copy of the License is located at http://aws.amazon.com/apache2.0/ or in the accompanying "license" file. This code is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either expressed or implied. See the License for specific language governing permissions and limitations.