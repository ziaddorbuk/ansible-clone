# ANSIBLE CLONE REPOS

## prerequisites:

Install ansible through the following [link](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

## Get Started: 

### Edit hosts.ini

Edit hosts.ini with your target hosts

### Create ansible vault

```
ansible-vault create vault.yml 
```
### Edit ansible vault
```
ansible-vault edit vault.yml
```
### content of the vault
```
github_token: ""
ansible_ssh_pass: ""
ansible_become_pass: ""
```

### Run playbook

```
ansible-playbook -i hosts.ini clone.yml --ask-vault-pass
```
