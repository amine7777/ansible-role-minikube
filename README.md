Ansible role: Minikube
=========

This role helps you to install minikube on your linux machine.


|Travis|CircleCI|GitHub|Quality|Downloads|Version|
|------|--------|------|-------|---------|-------|
|[![travis](https://travis-ci.com/amine7777/ansible-role-minikube.svg?branch=master)](https://travis-ci.com/amine7777/ansible-role-minikube)|![circleci](https://circleci.com/gh/amine7777/ansible-role-terraform.svg?style=svg)|[![github](https://github.com/amine7777/ansible-role-minikube/workflows/CI/badge.svg)](https://github.com/amine7777/ansible-role-minikube/actions)|[![quality](https://img.shields.io/ansible/quality/49942)](https://galaxy.ansible.com/amine7777/minikube)|[![downloads](https://img.shields.io/ansible/role/d/49942)](https://galaxy.ansible.com/amine7777/minikube)|[![Version](https://img.shields.io/github/release/amine7777/ansible-role-minikube.svg)](https://github.com/amine7777/ansible-role-minikube/releases/)|

![](minikube.jpeg)
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
```yaml
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
