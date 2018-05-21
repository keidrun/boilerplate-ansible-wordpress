# boilerplate-ansible-wordpress

Boilerplate of Ansible to create WordPress and MySQL.

## Let's get started !

- Clone this repository
- Prepare web server and db server
- Set host names to an `inventory` file
- Finally do the following commands

```bash
$ ansible -m ping all -i ./inventory
$ vi ./roles/wordpress/vars/main.yml
wp_mysql_host: X.X.X.X # Overwrite it to your db server's IP address
$ ansible-playbook playbook.yml -b -i ./inventory
```
