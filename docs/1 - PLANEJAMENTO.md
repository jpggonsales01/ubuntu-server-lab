# Planejamento do Projeto — Servidor de Arquivos Empresarial

## 1. Visão geral

Este projeto tem como objetivo desenvolver um **servidor de arquivos baseado em Ubuntu Server**, utilizando ferramentas gratuitas e de código aberto para oferecer uma solução segura, organizada e de baixo custo para pequenas e médias empresas.

A proposta é fornecer uma alternativa para empresas que não possuem condições financeiras para adquirir equipamentos NAS comerciais, como um Synology, utilizando hardware disponível ou de menor custo.

O servidor será responsável pelo **armazenamento, compartilhamento, gerenciamento de usuários, controle de acesso e backup dos dados**, além de disponibilizar uma interface web para facilitar a administração.

---

## 2. Objetivos

### Objetivo principal

Criar uma solução de servidor de arquivos empresarial com baixo custo, utilizando software livre, que permita:

* Armazenar arquivos da empresa de forma centralizada;
* Compartilhar arquivos através da rede;
* Criar e gerenciar usuários;
* Controlar permissões de acesso às pastas;
* Administrar o servidor através de uma interface web;
* Proteger o servidor utilizando firewall;
* Realizar backups automáticos;
* Monitorar os backups através de notificações por e-mail;
* Facilitar a manutenção e administração do ambiente.

### Objetivos secundários

* Reduzir a dependência de soluções NAS comerciais;
* Padronizar a implantação do servidor;
* Facilitar a administração para pessoas com pouco conhecimento de Linux;
* Criar uma documentação completa para futuras instalações;
* Desenvolver uma solução que possa ser replicada em diferentes empresas.

---

# 3. Tecnologias utilizadas

| Tecnologia         | Função                                                |
| ------------------ | ----------------------------------------------------- |
| Ubuntu Server      | Sistema operacional do servidor                       |
| Samba              | Compartilhamento de arquivos na rede                  |
| Cockpit            | Administração do servidor através de interface web    |
| 45Drives           | Gerenciamento de arquivos, pastas e compartilhamentos |
| UFW                | Firewall do servidor                                  |
| Script de Backup   | Automação dos backups                                 |
| SMTP/E-mail        | Notificação dos backups                               |
| Cron/Systemd Timer | Agendamento das tarefas automáticas                   |

---

# 4. Próximas etapas

A ordem planejada para desenvolvimento será:

* [ ] Instalar Ubuntu Server
* [ ] Configurar rede e hostname
* [ ] Atualizar o sistema
* [ ] Instalar Samba
* [ ] Criar estrutura de pastas
* [ ] Criar usuários e grupos
* [ ] Configurar permissões
* [ ] Criar compartilhamentos Samba
* [ ] Instalar Cockpit
* [ ] Instalar e configurar 45Drives
* [ ] Instalar e configurar UFW
* [ ] Desenvolver sistema de backup
* [ ] Configurar agendamento automático
* [ ] Implementar comparação entre backups
* [ ] Implementar notificações por e-mail
* [ ] Realizar testes de segurança
* [ ] Realizar testes de backup e recuperação
* [ ] Finalizar documentação
* [ ] Preparar o projeto para implantação em empresas
