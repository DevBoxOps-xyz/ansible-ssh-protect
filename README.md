# ssh-protect

Role for disabling ssh password authorization and setting the i attribute on the file `/root/.ssh/authorized_keys`.

## Deploy example

```yaml
  roles:
    - role: ssh-protect
      ssh_protect_root_public_keys:
        - KEY1
        - KEY2
        ...
        - KEYN
```

## Available parameters

### Main

| Param | Default | Description |
| -------- | -------- | -------- |
| `ssh_protect_root_public_keys` | `-` | Root ssh keys. |
