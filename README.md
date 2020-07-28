Minikube
=========

This role helps to install minikube on your linux machine.
![badge](https://action-badges.now.sh/amine7777/install_minikube)
[![Actions Status](https://github.com/amine7777/install_minikube/workflows/ci/badge.svg)](https://github.com/amine7777/install_minikube/actions)

Requirements
------------
- Linux machine
- Ansible 2.9

Role Variables
--------------
These variables helps to manage minikube installation.

You can specify your minikube version in this variable.
```yaml
minikube_version: latest
```
This is the url where minikube will be downloaded.
```ỳaml
minikube_download_url: "https://storage.googleapis.com/minikube/releases/{{ minikube_version }}/minikube-linux-amd64"
```
This is the path where minikube binary will be stored.
```yaml
minikube_dir_path: /usr/local/bin
```

Example Playbook
----------------

```yaml
- hosts: all
  roles:
     - amine7777.minikube
```

Author Information
------------------

- [Amine Kahlaoui](https://github.com/amine7777), DevOps engineer.
