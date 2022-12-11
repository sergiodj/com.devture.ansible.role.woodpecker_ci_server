# Woodpecker CI Server Ansible role

This is an [Ansible](https://www.ansible.com/) role which installs the **server** component of [Woodpecker CI](https://woodpecker-ci.org/) to run as a [Docker](https://www.docker.com/) container wrapped in a systemd service.

This role *implicitly* depends on [`com.devture.ansible.role.systemd_docker_base`](https://github.com/devture/com.devture.ansible.role.systemd_docker_base).

The **agent** component of Woodpecker CI is managed by a sibling role - [com.devture.ansible.role.woodpecker_ci_client](https://github.com/devture/com.devture.ansible.role.woodpecker_ci_client).

For an examply playbook that wires both Woodpecker CI **server** and **client** with a Postgres database and a Gitea version-control system, you can get inspiration from [gitea-docker-ansible-deploy](https://github.com/spantaleev/gitea-docker-ansible-deploy)'s `setup.yml` and `group_vars/gitea_servers` files.
