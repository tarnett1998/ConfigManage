## Apache Security Checks Playbook

### Usage

- Edit the `inventory.ini` file to have the correct IP addresses
- Edit the `hosts` entry in `sec_playbook.yml` to what destination to target
- Run: `ansible-playbook -i inventory.ini sec_playbook.yml -K` and enter the sudo password

### Security Checks - Web Config

The playbook will error out if it does not find specific lines in target config files. Make those changes and then run the playbook again.

### Security Checks - Network Sec

This will check for open ports + firewall rules. It will update the firewall with new rules. 

### Security Checks - User Sec

This will check for all users on the machine and make sure PAM authentication is secure.

### Security Checks - SSH Sec

This wil check to make sure the sshd configuration file does not contain potential security flaws.
