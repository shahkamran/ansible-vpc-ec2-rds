# Ansible to create VPC, Networks, EC2 Instance and RDS
Setting up AWS infrastructure with a Bastian server and RDS within its dedicated VPC and associated elements.

# Objectives
In this repository you will be carrying out following tasks in automated way.
 * Create a new VPC
 * Create VPC Subnets
 * Create VPC Routes
 * Create Security Groups
 * Create EC2 Instance
 * Create RDS Instance
 * Clean-up to terminate all above

# Prerequisites
You must have following before running this playbook.
 * AWS Account
 * AWS IAM Security Key and credentials
 * AWS EC2 Key Pair
 * A Linux computer or instance with Ansible, Git and required Python tools installed.
 * This repository
 
# How to

 * Add AWS Security Key credentials to ~/.boto file.
 * Create a new EC2 Key Pair and secure the private key.
 * Download repository using "git clone repositoryURL" command.
 * Amend variables listed in group_vars/all/vars and add your settings or preferences.
 * If you want RDS creation modify site.yml and uncomment RDS role. Please note RDS creation takes up to 30 minutes and incurs additional charges.
 * To provision infrastructure run "ansible-playbook site.yml".
 * To clean-up and terminiate your infrastructure you can run "ansible-playbook destroy.yml".

# Enjoy
Simple as that.
