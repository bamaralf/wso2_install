Role Name
=========

This Ansible role installs WSO2 products from repacked zip files.

Requirements
------------
It requires that you repack the zip file obtained from http://wso2.com with the source folders placed directly under the root folder instead of product_folder > source folders.
When you unzip the repacked folder you should get the source folders outside of any folder.

Role Variables
--------------
Please check test/test.yml

Dependencies
------------
Java JDK

Example Playbook
----------------
test/test.yml

License
-------

Apache

Author Information
------------------

Bruno Amaral
