Role Name: Slaves
=========

In this role of Slaves you will find how we can configure the Slaves on the AWS instances. 

Role Variables
--------------

The variable of the **master_token** will receiving the tokens after the initialization of the master node. The variable **master_token** is used inside the tasks of the slaves inside the *Joining Slaves to Master Node*.


Modules and Parameters Used:
------------
1. hosts
2. tasks
3. package
4. service
5. ignore_errors
6. changed_when
7. register
8. debug


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters):
```
- hosts: ["tag_Name_K8S_Slave1_testing", "tag_Name_K8S_Slave2_testing"]
  vars_prompt:
     - name: "master_token"
       prompt: "Enter Token To Join To Master: "
       private: no
  roles:
     - name: "Configuring Slave Node"
       role:  "/root/MultiNodeK8SCluster/Slaves"
```
