Role Name: ec2_launch
=========

In this role, you will find the tasks in the tasks folder inside main.yml file. Where as the variable folder consists of variables that used thoughout the tasks.

Requirements
------------
## modules used:
ec2

Role Variables
--------------
The  below variables are used in the tasks. But you can see this variables in the vars folder also.
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
Os_Names       -- will take the names of the OS

```


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters):

    - hosts: "localhost"
      roles:
        - name: "Launching ec2-instance"
          role: "ec2_launch"

