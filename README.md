# Apex CLI

Este repositório contém a CLI oficial da Apex Monitoring Solutions, desenvolvida em Bash puro, com foco na administração de servidores Linux e integração com plataformas de monitoramento e automação como Zabbix, Ansible e SaltStack.

## Objetivo

A `apex-cli` foi projetada para ser uma ferramenta unificada de linha de comando que facilita a operação diária de ambientes monitorados. Ela permite que administradores executem tarefas localmente ou remotamente a partir de um host central, como:

- Coleta de métricas (CPU, disco, rede, memória, I/O)
- Diagnóstico de infraestrutura
- Instalação e gerenciamento do Apex Agent (Zabbix customizado)
- Execução de comandos remotos via SSH
- Aplicação de playbooks via Ansible
- Integração opcional com SaltStack

## Estrutura do Projeto

```text
/usr/local/bin/apexctl              # Binário principal da CLI
/usr/local/bin/apex.d/             # Módulos Bash individuais (comandos)
/etc/apexctl/                      # Arquivos de configuração da CLI
/usr/share/apexctl/scripts/       # Scripts auxiliares
/usr/share/apexctl/playbooks/     # Playbooks Ansible padrão
```
Cada comando é implementado como um script executável no diretório apex.d/.

---

## Requisitos

- Bash >= 4.0
- Ansible (para execução de playbooks)
- OpenSSH Client (para execução remota)
- `zabbix_sender` (opcional)
- `zabbix_get` (opcional)
- SaltStack (opcional)

---

## Instalação

- Clone o repositório:

```bash
git clone https://github.com/rsdenck/apex-cli.git
cd apex-cli
```
- Execute o instalador com permissões de superusuário:
```bash
sudo ./install.sh
```
---

## **Licença**

Este projeto está sob a Licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## **Contatos**

- **Nome:** Ranlens Denck
- **Empresa:** Apex Monitoring Solutions
- **Email:** ranlens.denck@protonmail.com


