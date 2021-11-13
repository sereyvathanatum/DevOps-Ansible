# Check ansible status
ansible all -m ping

# Syntax check
ansible-playbook {{playbook_file}} --syntax-check

# Apply configuration
ansible-playbook {{playbook_file}}