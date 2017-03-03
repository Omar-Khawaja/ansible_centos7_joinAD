This Ansible playbook joins CentOS 7 nodes to an Active Directory domain. 
The variables containing the domain name and domain admin's credentials are
kept in an encrypted file in group_vars/nodes/vault.

The vault-password is stored on the master node and is used to decrypt vault-encrypted
files. The location of the vault-password can be specified with the --vault-password-file
flag (ex: ansible-playbook site.yml --vault-password-file ~/.vault_pass.txt).

To learn more about using Ansible Vault, refer to Ansible's official documentation at
http://docs.ansible.com/ansible/playbooks_vault.html#vault
