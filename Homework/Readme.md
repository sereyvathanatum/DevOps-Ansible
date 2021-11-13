# Configure inventory
sudo nano /etc/ansible/hosts
[ansible_aws_demo]
175.41.163.182 ansible_ssh_user=admin ansible_ssh_private_key_file=~/Class/DevOps/vathana-ec2.pem

# Check ansible status
ansible all -m ping

# Syntax check
ansible-playbook {{playbook_file}} --syntax-check

# Apply configuration
ansible-playbook {{playbook_file}}