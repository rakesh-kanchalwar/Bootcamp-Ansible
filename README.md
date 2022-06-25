# Ansible script to setup weight-tracker app 
This ansible script installs following apps on the servers provided in the configurations:
- nodejs
- weight-tracker app
- pm2

## How to use
As a first step of configuring remote server, update the server details such as ip address, okta url and credentials in the variable files.
Then, execute below command,

```js
ansible-playbook site.yml -i environments/stage --ask-vault-pass
```
Here, vault password is required at the time of script execution as to decrypt the credentials present in the varialbe files.