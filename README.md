K8s-NodesPrep
=========
An Ansible role to prepare Kubernetes nodes before bootstrapping the cluster.

Requirements
------------
These are the requirements for this role:
- CentOS 7/8 virtual machines
- Preinstalled container run-time engine

Role Variables
--------------
- node_type: "master"|"worker" (type of node to prepare)
- ip_prefix: "x" (IP prefix of the primary interface)


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: masters
      roles:
         - { role: HosniNabil.K8s-NodesPrep, node_type: "master", ip_prefix: "24" }
    - hosts: workers
      roles:
          - { role: HosniNabil.K8s-NodesPrep, node_type: "worker", ip_prefix: "24" }
License
-------

Apache License 2.0

Author Information
------------------
Nabil Hosni, cloud engineer and opensource enthusiast.
