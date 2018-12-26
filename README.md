# Ansible Role: Shoutcast

#### Version: 1.0.0

Development of this project is managed in a private repository then pushed out to [GitLab](https://gitlab.com/sparknsh/ansible-role-shoutcast) and [GitHub](https://github.com/sparknsh/ansible-role-shoutcast) when we have a new version for you. If you have any issues please contact [sparknsh](https://www.sparknsh.com/contact?type=issue&name=ansible-role-shoutcast)

## Role Variables

```yaml
shoutcast_streams: []
```

#### Example

```yaml
shoutcast_streams:
  - port: 8000
    listeners: 10000
    passwd: 4W7APeAAv7w7jUt
    admin_passwd: y48DCnuE74RRSYVAWBjpWzXbL7brhe
    hash: dqp8cj2dZdXcdz1sazE3 # Optional
    extras:
      srcip: 10.99.0.50
    state: present

```

## Example Playbook

```yaml
- hosts: all
  vars_files:
    - vars/main.yml
  roles:
     - { role: sparknsh.shoutcast }
```

## License

MIT

## Author Information

This role was created in 2018 by [sparknsh](https://www.sparknsh.com) at [Rebel Media, Inc.](https://www.rebelmedia.io/)
