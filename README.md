# Fortiswitch-Ansible
Contains playbooks for configuring stand-alone Fortiswitches. 

Currently the following configuration is supported by the playbook:
- Settings system DNS
- Configuring a system interface
- Configuring a SNMPv3 user
- Configuring SNMP info
- Configuring NTP

The following is required to run playbooks from this repo:
- Ansible
- The Fortiswitch Ansible collection

Installation of these requirements can be done as follows:
```
apt install ansible -y
ansible-galaxy collection install fortinet.fortiswitch
```
Make sure to create a valid inventory file based on vars/hosts.example. 
Running the playbook goes as follows:
```
ansible-playbook -i vars/hosts-prod play-fortiswitch.yml
```
