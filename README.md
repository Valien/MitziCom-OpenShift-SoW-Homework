# MitziCom-OpenShift-SoW-Homework
Homework for the OpenShift Deployment Labs

Full homework instructions are [here](https://www.opentlc.com/labs/ocp_advanced_deployment/08_1_Assignment_Lab.html).

This is leveraging the casl-ansible project: https://github.com/redhat-cop/casl-ansible

* Engagement journal in .pdf format (F8F logos, SoW template, etc).
* Different PV types
* Default project templates - deny-by-default, then allowed... (isolated, etc.)
* Multi-tenancy - node-selectors, user objects, client objects (check docs) -- new user template (extra credit?!?)

** To Run **

* ssh to bastion host
* git clone
* `ansible -i $PWD/hosts masters --list-hosts` -- checks hosts file
* `ansible -i $PWD/hosts nodes --list-hosts` -- checks nodes
* `ansible -i $PWD/hosts all --list-hosts` -- all nodes/hosts
* `ansible -i $PWD/hosts all -m ping` -- ping all hosts

Export bastion guid:

* `export GUID=`hostname | cut -d"." -f2`; echo "export GUID=$GUID" >> $HOME/.bashrc`
* `echo GUID=$GUID`
