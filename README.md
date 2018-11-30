# MitziCom-OpenShift-SoW-Homework
Homework for the OpenShift Deployment Labs

Follow the steps below to start the OpenShift 3.11.16 POC installation:

1.	Clone this repo -  `git clone https://github.com/Valien/MitziCom-OpenShift-SoW-Homework.git`
2.	CD to the directory – `cd MitziCom-OpenShift-SoW-Homework/`
3.	CD to the playbooks directory – `cd playbooks/`
4.	Run the following command: `ansible-playbook -f 20 install_openshift.yaml --extra-vars "OREG_AUTH_USER=<INSERT RH USER> OREG_AUTH_PASSWORD=<INSERT RH PASSWORD"`
 
 ** You will need to put in your Red Hat username and password.

5.	The installation takes about 30 minutes. 
