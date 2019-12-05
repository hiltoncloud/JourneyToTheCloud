				What will be build
1. A wordpress blog will be built using AWS,Terraform and ansible.
				
			        Environment Setup
1. Python 2.7.12 or above required
2. Update the system
3. Install python-pip
4. pip install --upgrade pip
5. download terraform 
curl -O https://releases.hashicorp.com/terraform/0.11.2/terraform_0.11.2_linux_amd_64.zip
6. mkdir /bin/terraform
7. unzip the terraform into that new folder use the -d flag to specify the new directory you just created.
8. Next Add teraform to your path. export PATH=$PATH:/bin/terraform

				Install AWS CLI'
9. pip install awscli --upgrade
10. check if its installed "aws --version"
11. run update
12. apt-get install software-properties-common
				Install Ansible
13. apt-add-repository ppa:ansible/ansible
14. apt-get update
15. apt-get install ansible 
16. ansible --version
				Generate A Keygen to access servers
17. ssh-keygen
18. Destination: /root/.ssh/journeytothecloud
19  ssh-agent bash
20. ssh-add ~/.ssh/journeytothecloud
21. ssh add -l to ensure it is there
22. Run steps 19-21 everytime you begin production

23.				Modify the ansible File,
because aws is not hosting your access key you need to disable host key checkingin the ansible file use the search command to find host_key_checking

etc/ansible/ansible.cfg

24. make a working_directory "working_dir_terraform_ansible"
25. move into directory.


