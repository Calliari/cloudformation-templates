### Cloudfromation-template


The `aws_cf_project_automation_vpc.yml` would create resources as the following:

- vpc
- SubnetPublic0:
- SubnetPrivate1:
- InternetGateway:
- VPCGatewayAttachment:
- PublicRT:
- PrivateRT:
- NATElasticIP:
- NATGateway:
- NATGatewayRoute:
- RoutePublicNATToInternet:
- NATGatewayRoute:
- RouteTableAssociationPublic:
- RouteTableAssociationPrivate:
- BastionSecurityGroup:


- Outputs:
    - Description: The ID of the VPC
    - Description: The SubnetPublic of the VPC
    - Description: The SubnetPrivate of the VPC
    - Description: The Bastion Security Group of the VPC
    
    
    
The `aws_cf_project_automation_ec2.yml` would create resources as the following:
 - a bastion ec2 based on the `aws_cf_project_automation_vpc.yml` 

Using the VPC, subnets and etcs as well as importing the exposed outputs from the template. This is nested-template or another name for it cross-template strategy.
