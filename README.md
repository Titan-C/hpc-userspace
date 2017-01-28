# hpc-userspace
Ansible playbook to install software in computing cluster in userspace

This project came to realization as I was not able to get the
administrators of my cluster to install recent software so that I
could compile and run the software I need to do my calculations.

Thus with no better alternative than installing my dependencies in
userspace to get things working, I wrote this playbooks.

This is in the limit of an automation script and a very bad package
manager.

To run everything

```bash
ansible-playbook -i ./machines site.yml -vv
```

To run a specific component, `htop` for example.

```bash
ansible-playbook -i ./machines site.yml --tags htop -vv
```
