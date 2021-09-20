# Apache Security Checks Playbook

## Usage

- Edit the `inventory.ini` file to have the correct IP addresses
- Edit the `hosts` entry in `sec_playbook.yml` to what destination to target
- Run: `ansible-playbook -i inventory.ini sec_playbook.yml -K` and enter the sudo password