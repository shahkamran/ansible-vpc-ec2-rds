# Ansible to create VPC, Networks, EC2 Instance and RDS
Setting up AWS infrastructure with a Bastian server and RDS within its dedicated VPC and associated elements.

# Prerequisites
You must have following before running this playbook.
 * AWS Account
 * AWS IAM Security Key and credentials for user account to be used in this project. Plase your credentials in .boto file in your home directory.
 * A Linux computer with Ansible, Git and required Python tools installed.
 * Download this repository using "git clone https://github.com/shahkamran/ansibleinfrastructuresetup.git"
 * AWS EC2 Key Pair Name required for these scripts. You should keep the private key safe.
 
# How to use this repository.
Once you have it all available you will have to amend variables in vars file located in group_vars/all/vars.

Once all variables are configured you can execute following to set it up all for you.
ansible-playbook site.yml

And when you finish it all, you can again run following to completey clean up everything created by previous script.
ansible-playbook destroy.yml

# Simple as that.
