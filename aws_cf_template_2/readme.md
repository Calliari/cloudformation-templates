
#### CloudFormation Blog Activity

The `aws_cf_template.yml.yml` `aws_cf_template.json` would create resources as the following:

Iy would create a high available infra with all neccesssary resources for a wordpress blog web-site and exposed as outputs the private Ip adrdress and well as the public Ip address.

Resources:
  - VPC
  - InternetGateway
  - VPCGatewayAttachment
  - DMZ1public
  - DMZ2public
  - AppLayer1private
  - AppLayer2private
  - PublicRT
  - RouteTableAssociationA
  - RouteTableAssociationB
  - RoutePublicNATToInternet
  - NATElasticIP
  - NATGateway
  - NATGatewayRoute
  - PrivateRT
  - RouteTableAssociationC
  - RouteTableAssociationD
  - DMZNACL
  - SubnetNetworkAclAssociationA
  - SubnetNetworkAclAssociationB
  - DMZNACLEntryIngress100
  - DMZNACLEntryIngress110
  - DMZNACLEntryIngress120
  - DMZNACLEntryIngress130
  - DMZNACLEntryEgress100
  - DMZNACLEntryEgress110
  - DMZNACLEntryEgress120
  - DMZNACLEntryEgress130
  - AppNACL
  - SubnetNetworkAclAssociationC
  - SubnetNetworkAclAssociationD
  - AppNACLEntryIngress100
  - AppNACLEntryIngress110
  - AppNACLEntryIngress120
  - AppNACLEntryIngress130
  - AppNACLEntryEgress110
  - AppNACLEntryEgress120
  - AppNACLEntryEgress130
  - LoadBalancer
  - Listener
  - TargetGroup
  - BastionSecurityGroup
  - LoadBalancerSecurityGroup
  - WebServerSecurityGroup
  - LaunchConfiguration
  - AutoScalingGroup
  - BastionInstance

 - Outputs:
    - Description: Public ip address of bastion instance
    - Description: Private ip address of bastion instance
