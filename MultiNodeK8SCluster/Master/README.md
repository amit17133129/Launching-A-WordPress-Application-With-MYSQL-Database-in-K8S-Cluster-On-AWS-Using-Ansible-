Role Name: Master
=========

In this role of Master,  you will find that how we can configure the master on AWS instance.

Role Variables
--------------

You need to copy the tokens generated in the ***Generating Token*** section of the playbook

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
- hosts: ["tag_Name_K8S_Master_testing"]
  roles:
  - name: "Configuring Master Node"
    role:  "/root/MultiNodeK8SCluster/Master"
```


