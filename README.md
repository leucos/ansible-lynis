# Ansible Role: Lynis

An Ansible Role that installs Lynis (community or customer)
Debian/Ubuntu Linux.

## Role Variables

Available variables are listed below. All of them are optional. Thus No
default values are set.

  - `lynis_licence_key`: your customer licence key if running customer
    version (see https://cisofy.com/ for more information).
  - `lynis_system_customer_name`: name of customer for system (customer
    version)
  - `lynis_tags`: list of tags to apply to host
  - `lynis_skip_tests`: list of tests to skip
  - `lynis_cron`: whether to add a lynis daily cron (customer version
    only supported for now)

## Dependencies

None.

## Example Playbook

    - hosts: webservers
      roles:
        - { role: leucos.ansible-lynis }

## License

MIT / BSD

## Author Information

[leucos](https://github.com/leucos).

