# Playbook para instalar AWX en CentOS 8/9
## Iniciar el playbook con:

```bash
ansible-playbook -i inventory/hosts.yml OS-CENTOS-ansible-playbook.awx.dockercompose.install.yml --ask-become-pass
```

ó

```bash
ansible-playbook -i inventory/hosts.yml OS-CENTOS-ansible-playbook.awx.dockercompose.install.yml --ask-become-pass --extra-vars "awx_admin_password=ejemplo"
```

Asegurarse de tener el agente ssh
```bash
eval "$(ssh-agent -s)"
ssh-add
```