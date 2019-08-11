### cloudformation template  - IAM Role for S3

This cf would create a infra to have access to a s3 bucket from a ec2 using roles;

Resources:
- EC2
- EC2WithRole profile 
- security group with port 22 open to everywhere [0.0.0.0]
- S3BucketPolicy attached to the bucket ('List' and 'CreateBucket' buckets permission only)
- S3BucketRole attached to ec2
- Outputs
     - Description: EC2 connect string to ssh into ec2 E.X(ssh ec2-user@3.85.172.254 -i tempkey.pem)


<hr></hr> 
SSH into ec2:

`ssh ec2-user@3.85.172.254 -i tempkey.pem`

And run:
- `sudo yum update` to update all software packages
- `aws s3 ls` one bucket will be listed as part of the cloudformation
- `aws s3 mb s3://testbucket-mybucket` create a new bucket (buckets' need to be global unique so change the name if it's failed to creta a bucket with this name)
- `aws s3 ls` now there are 2 buckets
