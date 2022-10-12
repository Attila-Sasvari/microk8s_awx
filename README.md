# Synopsis

The repository is a GitHub project that includes roles and a playbook to install `Microk8s`, then deploy `AWX` on it, finally configure AWX with some project, job template, etc.

```json
This asset is not ready for usage!
The project includes the skeleton of the asset with some well-defined tasks, but it's not finished or tested.
It's acceptable to demonstrate the planned solution to the problem.
```

## Install Microk8s

The name of the related role: `install_microk8s`.

Its main workflow:
- Install docker.
- Install microk8s.
- Add user to the required groups and perform a few additional configuration.

Note: alternative solution would be to utilize https://galaxy.ansible.com/racqspace/microk8s.

## Deploy AWX

The name of the related role: `deploy_awx`.

Its main workflow:
- Deploy AWX operator.
- Access AWX admin password and URL.

Note: alternative solution would be to utilize https://galaxy.ansible.com/racqspace/awx.

## Configure AWX

The name of the related role: `config_awx`.

Its main workflow:
- Add a team and a user.
- Add a project.
- Add an inventory.
- Add credentials.
- Add job templates.

This role highly relies on the variables created in the `vars/` directory.
