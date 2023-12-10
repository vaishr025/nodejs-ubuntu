# Ansible Vault Usage and Playbook Execution

This guide demonstrates how to create and use an Ansible Vault file to securely store sensitive information and how to run Ansible playbooks that utilize encrypted variables.

## Generating an Ansible Vault File

1. **Create a new Vault file:**

   ```bash
   vi ansible-vault create vault_secret.yml

  1.1 Enter a password for the Vault file when prompted.

2.  ** Provide following contents to vault_secret.yml**

   user_name:
   user_password:

3. Save the password 

## Executing playbook 

ansible-playbook -i inventory_file node_app_setup.yml --ask-vault-pass

Please provide the vault password when prompted for password usage
