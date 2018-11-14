
# kitchen-travis test
Kitchen-vagrant test that checks the vagrant virtualbox box have redis

## pre-requirements

all pre-requirementa to make this work here:
- Linux OS Ubuntu 18.04
- Install **Vagrant**
    - Download and install accordingly to your OS as described here : https://www.vagrantup.com/downloads.html

- Install **Ruby environment**
			```
- Install **Packer**
    - Download and install accordingly to your OS as described here : https://www.packer.io/downloads.html
 - Install **Virtualbox**
	 - Follow the instruction from: https://www.virtualbox.org/wiki/Downloads

## How to run the code
In the terminal run the following commands:
	
	packer build template.json
	vagrant box add --name nginx --provider virtualbox vagrant box ubuntu-1604-vbox.box
	kitchen init
	kitchen list
	kitchen converge
	kitchen verify
	kitchen destroy
