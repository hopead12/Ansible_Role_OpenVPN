My a little Ansible role

Requirements
------------

For instance, must write to instance ip file in hosts.txt and write to path to ssh key in group_vars/Prod

Role Variables
--------------

The only destin_file variable is /usr/local/openvpn_as/etc in defaults/main.yml

Example Playbook
----------------

- name: OpenVPN install on Ubuntu
  hosts: Prod
  become: yes

  roles:
   - deploy_my_openvpnas