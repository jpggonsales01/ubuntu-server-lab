## Primeira etapa – Instalar e configurar Ubuntu/Samba

### Objetivo

Criar um servidor de arquivos utilizando **Ubuntu Server** e **Samba**, permitindo acesso compartilhado a partir de computadores **Windows**.

---

### Ambiente utilizado

* **Virtualizador:** VirtualBox
* **Sistema operacional:** Ubuntu Server 26.04 LTS
* **Link para download do VirtualBox:** https://www.virtualbox.org/wiki/Downloads
* **Link para download do Ubuntu Server:** https://ubuntu.com/download/server

---

### Configuração inicial da máquina virtual

| Recurso     | Configuração                                |
| ----------- | ------------------------------------------- |
| Memória RAM | 2 GB                                        |
| Processador | 1 vCPU                                      |
| Disco       | Dinâmico                                    |
| Rede        | Bridge                                      |

**Observação:** inicialmente configurei a VM com recursos mínimos apenas para testes e monitoramento de consumo. A ideia é aumentar CPU e memória conforme o projeto evoluir.

---

### Instalação do Ubuntu Server

Após baixar a ISO do Ubuntu Server:

1. Criei uma nova máquina virtual no VirtualBox.
2. Configurei a ISO como mídia de boot.
3. Realizei a instalação padrão do Ubuntu Server.
4. Defini usuário, senha e hostname da máquina.

---

### Instalação do Samba

Com o Ubuntu já configurado, iniciei a instalação do Samba utilizando os comandos abaixo:

```bash
sudo apt update
sudo apt install samba -y
```

Verificação do serviço:

```bash
sudo systemctl status smbd
```

---

### Resultado da etapa

* Ubuntu Server instalado com sucesso.
* Acesso ao terminal funcionando normalmente.
* Samba instalado e serviço **smbd** ativo.

# Segunda etapa - Instalação do pacote Cockpit para visualização fácil de consumo e manejo de arquivos

Escolhi o Cockpit, pois é uma interface que nunca utilizei antes. Irei testar a funcionalidade temporariamente. Se eu não me adequar, voltarei a utilizar o Webmin.

## Instalando o pacote

Antes de qualquer comando, atualizo a lista de pacotes com:

```bash
sudo apt update
```

Após isso, começo instalando o Cockpit:

```bash
sudo apt install cockpit -y
```

Com o Cockpit instalado, vou ativar e iniciar o serviço:

```bash
sudo systemctl enable --now cockpit.socket
```

Para testar se o serviço está ativo:

```bash
sudo systemctl status cockpit.socket
```

Agora, sabendo que o Cockpit está realmente ativo, vou para o teste real e acesso a interface web utilizando o endereço IP e a porta:

```text
http://192.168.100.176:9090
```

Conferi o funcionamento da interface. Em uma configuração futura, alterarei a porta padrão utilizada pelo Cockpit e ajustarei as regras do firewall para permitir o novo acesso
