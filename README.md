Minikube
=========

This role helps to install minikube on your linux machine.

Requirements
------------
- Linux machine
- Ansible 2.9

Role Variables
--------------
These variables helps to manage minikube installation.

```yaml
minikube_version: latest
minikube_download_url: https://storage.googleapis.com/minikube/releases/{{ minikube_version }}/minikube-linux-amd64
minikube_dir_path:  /usr/local/bin
```

Example Playbook
----------------



    - hosts: all
      roles:
         - { role: amine7777.minikube }


Author Information
------------------

- [Amine Kahlaoui](https://github.com/amine7777), DevOps engineer.
