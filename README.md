## Drupal+Nginx+PHP-FPM+MariaDB Deployment

- Requires Ansible 1.2 or newer
- Expects CentOS/RHEL 7.x host/s

RHEL7 version reflects changes in Red Hat Enterprise Linux and CentOS 7:
1. Network device naming scheme has changed
2. iptables is replaced with firewalld
3. MySQL is replaced with MariaDB

Then run the playbook, like this:

	ansible-playbook -i hosts site.yml

The playbooks will configure MariaDB, Nginx, and PHP-FPM. Also prepares the server
for Drupal Installation and CiviCRM.
