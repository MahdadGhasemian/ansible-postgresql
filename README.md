# Ansible Role: Postgresql

Ansible galaxy role can run a postgresql on a docker container

## Requirements

None.

## Role Variables
```yaml
docker_postgres__name: postgres
docker_postgres__image: "postgres:15.3"
docker_postgres__port: 5432
docker_postgres__superuser_name: "postgres"
docker_postgres__superuser_password: "password"
docker_postgres__remove_existing_container: yes
docker_postgres__pull_image: yes
docker_postgres__home: "/root/postgresql"
docker_postgres__network_mode: "postgresql_network"
```

## Dependencies

- community.docker

## Example Playbook (using default package)

    - hosts: servers
      roles:
        - role: MahdadGhasemian.ansible-postgresql

## License

MIT / BSD

## Author Information

This role was created in 2023 by [Mahdad Ghasemian](https://mahdad.me/).