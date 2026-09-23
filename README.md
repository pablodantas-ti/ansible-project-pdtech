________________________________________
📄 README.md
# 🚀 Ansible Project - PDTECH
Projeto de automação utilizando Ansible para gerenciamento de servidores Linux, com foco em boas práticas de DevOps e Infraestrutura como Código (IaC).
---
## 📌 Objetivo
Automatizar:
- Provisionamento de serviços (Apache / Nginx)
- Aplicação de patches (updates)
- Validação de ambiente (uptime, status, updates)
- Organização de infraestrutura com roles e grupos
---
## 🧱 Estrutura do Projeto
ansible-project/
├── inventory/
│ ├── hosts.yml
│ └── group_vars/
├── roles/
│ ├── apache/
│ └── nginx/
├── playbooks/
│ ├── apache.yml
│ ├── nginx.yml
│ ├── patch.yml
│ └── check.yml
├── ansible.cfg
└── README.md
---
## ⚙️ Tecnologias Utilizadas
- Ansible
- Linux (Debian/Ubuntu)
- SSH
- Git / GitHub
---
## 📡 Inventário
Estrutura baseada em grupos:
- `webservers` → todos os servidores web
- `web_servers_apache` → servidores com Apache
- `web_servers_nginx` → servidores com Nginx
---
## ▶️ Playbooks
### 

🔹 Instalar Apache
ansible-playbook playbooks/apache.yml
🔹 Instalar Nginx
ansible-playbook playbooks/nginx.yml
🔹 Aplicar patches (update geral)
ansible-playbook playbooks/patch.yml
🔹 Validar ambiente (uptime + updates)
ansible-playbook playbooks/check.yml
________________________________________
🔐 Segurança
•	Acesso via SSH com chave pública
•	Usuário padrão: ansible
•	Uso de sudo sem senha para automação controlada
•	Arquivo hosts.yml não versionado (evita exposição de IPs)
________________________________________
🧪 Funcionalidades implementadas
•	✔️ Automação de instalação de serviços
•	✔️ Organização por roles
•	✔️ Inventário estruturado
•	✔️ Aplicação de patches automatizada
•	✔️ Validação de ambiente com fail em caso de inconsistência
________________________________________
👨‍💻 Autor
Pablo Dantas
Infraestrutura | Cloud | DevOps 
________________________________________
📎 Observações
Este projeto faz parte de estudos práticos em automação e boas práticas de infraestrutura.
