# Neo4j_Ansible

With this repository, Elastic Team creates the appropriate environment, using ansible
to deploy Neo4j distributed Graph database for the needs of the postgraduate
course ­ [M123 Distributed Systems](http://www.cslab.ntua.gr/~dtsouma/M123-DistrSys-spring2016.html).


# Provisioning

In the Provisioning phase, Elastic Team installs the appropriate software to the master node.

More specifically, in the environment has been installed the following:

* elastic-team (User / Group)
* Java 8 (jre)
* Neo4j


# Installation

- Copy your ssh keys to the remote hosts

  > ssh-copy-id root@host

- Make sure that you can ping you remote hosts

  > ansible all -i hosts -m ping -u root

- Install all the packages

  > ansible-playbook -i hosts elastic-team.yml
