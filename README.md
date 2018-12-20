# Ansible Packer
Install Packer with Ansible

## Install
Add to ```roles/requirements.yml```
```yaml
- src: git@github.com:thomaslorentsen/ansible-packer.git
  scm: git
  version: master
  name: thomaslorentsen.packer
```
and then run:
```bash
ansible-galaxy install -r roles/requirements.yml
```
## Usage
```yaml
- hosts: localhost
  roles:
    - { role: thomaslorentsen.packer, packer_version: "1.3.3" }
```
