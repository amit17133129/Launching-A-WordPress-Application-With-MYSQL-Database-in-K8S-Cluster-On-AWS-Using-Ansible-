Role Name: create_vpc
=========

This role will create the vpc on your respective AWS account.


Modules and Parameters Used:
------------

1. tasks         
2. ec2_vpc_net   -- For creating vpc
3. ec2_vpc_igw   -- For creating Internet Gateway
4. ec2_vpc_subnet-- For creating Subnets
5. ec2_group     -- For creating Security Group
6. ec2_vpc_route_table  -- Creating Route Table
7. debug
8. register


Role Variables
--------------
```
aws_access_key -- will take access key
aws_secret_key -- will take secret key
vpc_title      -- reference variable that will store the title
vpc_name       -- name of the vpc
igw_name       -- name of the internet gateway
subnet_name    name of subnet
security_group_name  -- name of security group
route_table_name  -- name of the routing table
vpcCidrBlock    -- cidr block of vpc
subNetCidrBlock  -- cid block of subnet
port22CidrBlock  -- cidr block
destinationCidrBlock -- destination cidr block
state          -- enter state
zone           -- enter availability zones
region         -- enter region
```


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

      - hosts: "localhost"
        roles:
          - name: "Creating VPC"
            role: "/root/create_vpc" 
