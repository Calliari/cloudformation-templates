# cloudformation-templates

#### aws_cf_template dir have templates to create a VPV. (The templates are in yml and json format)
These templates are the same but one writeen in JSON and the another in YML.
The templates will create the following resources:
- VPC: 1
- public subnets: 2
- private subnets: 2
- internate gateway: 1
- NAT gateway: 1
- a route table actached to a private subnet: 1
- a route table attadhed to a public subnet: 1
- the ACLs for each subnet created


#### aws_cf_template_1 dir contain a template to create a VPC and an ec2
- 1 create a VPC with a vpc template (aws_cf_project_automation_vpc.yml)
- 2 use the template which will need three parameters to create an ec2 intance based on the previous template. (aws_cf_project_automation_ec2.yml)


