Role Name
=========

This Ansible role installs WSO2 products from repacked zip files.

Requirements
------------
It requires that you repack the zip file obtained from http://wso2.com with the source folders placed directly under the root folder instead of product_folder > source folders. When you unzip the repacked folder you should get the source folders outside of any folder. Observation: This role doesn't encrypt any password, it only installs the products on its defaults   

Since version 6.0.0 the WSO2 integrator product contains:
esb, dss and msg-broker, but it's possible to install each product
on separated instances. If you need to do so, just run the playbook
with the accordingly PRODUCT_NAME. If you want to install the
integrator with all products on the same instance, you could use "esb" or "dss"
as PRODUCT_NAME and you will have the complete integrator install. The "msg-broker"
has a separated folder and start scripts that are under the integrator root folder
and you should use it on PRODUCT_NAME if you want to install specifically it.

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
