# hpc-userspace
Ansible playbook to install software in computing cluster in userspace

Although the power of ansible is the idempotence. I got so frustrated
checking the versions of installed packages in userspace that I rather
pick the package I want to update and call it by the tags.

```bash
ansible-playbook -i ./machines site.yml --tags gcc
