# Ansible1
- name: update yum package to rhel server
  hosts: all
  become: true
  tasks:
    - name: rhel server
      yum:
        name: "httpd"
        state: latest
