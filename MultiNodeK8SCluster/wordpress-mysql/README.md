Role Name: wordpress-mysql
=========

This Role will helps you to launch the pods of wordpress and mysql as well as it will expose the wordpress pod.



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: "Master Tag Name eg tag_Name_K8S_Master_testing"
      roles:
           - name: "Launching Wordpress and Mysql"
             role: "/root/MultiNodeK8SCluster/wordpress-mysql"
