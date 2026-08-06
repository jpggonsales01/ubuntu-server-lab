# Firewall UFW

Como estou lidando com um laboratório, inicialmente decidi utilizar o firewall UFW com pequenos ajustes.

## Verificando o status do UFW

Para verificar o status atual do firewall, utilizo o seguinte comando:

```bash
sudo ufw status
```

## Ativando o UFW

Após a verificação, ativo o firewall com o comando:

```bash
sudo ufw enable
```

## Liberando a porta do Cockpit

Por conta do repositório Cockpit, preciso abrir a porta utilizada para acessá-lo via web. Para isso, utilizo o comando:

```bash
sudo ufw allow 9090/tcp
```

## Liberando a porta SSH

Por último, libero a porta 22, padrão de acesso via protocolo SSH. Posso utilizar qualquer um dos comandos abaixo:

```bash
sudo ufw allow ssh
```

ou

```bash
sudo ufw allow 22/tcp
```
