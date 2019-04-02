Terraform
=========

Role to install (download) Terraform.


Role Variables
--------------

The role will try to load the variable file base on the host's OS feel free to
add additional files to include more systems.


vars/{{ ansible_system }}.yml

```
terraform:
 src_file_url: https://releases.hashicorp.com/terraform/0.11.13/terraform_0.11.13_linux_amd64.zip
 src_file_sha256: 5925cd4d81e7d8f42a0054df2aafd66e2ab7408dbed2bd748f0022cfe592f8d2
```


Example Playbook
----------------

```
- hosts: servers
  roles:
   - terraform
```


Author Information
------------------

Tal Lannder

tal@tal.fyi
