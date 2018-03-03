A Cloudformation template using Chef to automate the installation of WordPress..

Objective:
Use CM tools such as Puppet, Ansible, or Chef to automate the installation of basic Drupal or WordPress. Setup a sample site. Automate the solution using Cloudformation template.

Deliverable:
A CloudFormation template available in Git Repository (https://github.com/midebell/Rean-Chef-WP-VPC):
This template is named "CloudFormation_WP_VPC_Chef.JSON". When run, this will install:
VPC
EC2 Instance
Security Group
Subnet
Route Tables
IGW
NAT
EIP
And finally launch Chef CM (local mode) to configure WordPress through s3 recipe url.

Major Bumps:
Although the stack was completed, I could not see the wordpress site by launching the IP Address assigned.
Assumption is that you would need RDS with ELB and Autoscaling to make this work properly as contained in AWS reference at:

https://s3-us-east-2.amazonaws.com/cloudformation-templates-us-east-2/WordPress_Chef.template
https://sookocheff.com/post/aws/how-to-create-a-vpc-using-cloudformation     
https://s3-us-west-2.amazonaws.com/cloudformation-templates-us-west-2/VPC_Single_Instance_In_Subnet.templa
