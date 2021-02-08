Role Name: Provisioning Ec2 Instances
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
# vars file for ec2_launch
-- aws_access_key: 'enter your access key'
-- aws_secret_key: 'enter your secret key'
-- vpc_title: 'K8S Cluster'
-- vpc_name: "{{ vpc_title }} VPC"
-- igw_name: "{{ vpc_title }} IGW"
-- subnet_name: "{{ vpc_title }} Subnet"
-- security_group_name: "{{ vpc_title }} Security Group"
-- route_table_name: "{{ vpc_title }} route table"
-- vpcCidrBlock: '10.0.0.0/16'
-- subNetCidrBlock: '10.0.1.0/24'
-- port22CidrBlock: '0.0.0.0/0'
-- destinationCidrBlock: '0.0.0.0/0'
-- state: "present"
-- zone: "ap-south-1a"
-- region: "ap-south-1"
-- Os_Names:
     - "K8S_Master_testing"
     - "K8S_Slave1_testing"
     - "K8S_Slave2_testing"
```


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters):

    - hosts: "localhost"
      roles:
        - name: "Launching ec2-instance"
          role: "ec2_launch"

