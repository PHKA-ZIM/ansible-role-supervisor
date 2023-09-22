# Supervisor installation automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-supervisor
  name: ansible-role-supervisor
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-supervisor

- Import role and override role variables, e.g.
```
- name: Setup supervisor
  roles:
    - role: ansible-role-supervisor
```

- All available role vars can be found in `defaults`
