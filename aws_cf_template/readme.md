## cloudformation-templates

The two templates would create thesame resources they are just in different format one in JOSON and another in YAML; 

- `aws_cf_vpc_automation.json` 
- `aws_cf_vpc_automation.yml`


#### resources that would be created and two outputs that exposing some resoiurtces, can be used as cross-template or nested-template
- VPC: 1
- public subnets: 2
- private subnets: 2
- internate gateway: 1
- NAT gateway: 1
- a route table actached to a private subnet: 1
- a route table attadhed to a public subnet: 1
- the ACLs for each subnet created
- exporting StackName & VPC-ID
