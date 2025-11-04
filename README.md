# Midnight Miner Anisible

This is a simple Ansible playbook to deploy the Midnight Miner on a set of servers.

# Usage

Create a hosts.ini file with the servers you want to deploy the Midnight Miner to.

Should look like this:

```
[midnight_miners]
ip1
ip2
...
```

Create a .env file with the variables you want to use in the root directory.


Make sure to set the server_url in the group_vars/all.yml file.


Run the playbook with:
```
ansible-playbook -u root --key-file ./path/to/ssh_key.ppk site.yml
```