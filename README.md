# Preparação de Workstation Linux padrão

>**_Isenção de Responsabilidade_**:
> Esse scripts está relacionado a execução no Ubuntu 20.04, para outras distribuições, necessário adaptá-lo.

## Preparando Workstation
> Leia o arquivo `install.yml` antes de aplicá-lo e entada tudo qe será feito

1. Execute um update e instale o Ansible e git
```bash
sudo apt update && sudo apt install ansible git -y
```
2. Clone o repositório
```bash
git clone https://github.com/eglysc/DevOps.git
```

3. Execute a configuração
```bash
ansible-playbook tools/install.yml --ask-become-pass
```
>Digite sua senha quando solicitado a dar permissões de root para algumas ações.