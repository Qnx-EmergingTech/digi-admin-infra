# digi-admin-infra

1. Set the repository secret for SSH_PRIVATE_KEY and VAULT_PASSWORD

2. Update the inventory file for the server ip

3. Clone this repository inside the server as `deploy` directory

4. Run the action to verify the configuration



#### Install ansible

```sh
sudo apt install ansible-core
```

#### Deploy Admin

```sh
ansible-playbook playbook/deploy_admin_dev.yml -i playbook/inventory.yml
```

#### Stop admin

```sh
ansible-playbook playbook/stop_admin_dev.yml -i playbook/inventory.yml
```




