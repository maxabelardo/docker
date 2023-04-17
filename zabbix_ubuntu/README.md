# Zabbix

## Objetivo:
Esta imagen está sendo criada para facilitar a implantação de um servidor de monitoramento em cliente que não possui este recurso configurado em seu park. A imagen está pronta para ser inserida na rede do cliente, ficando apenas as configurações dos hosts no monitoramento.

## Como será feito este monitoramento?
Será criada uma imagen no docker com o Linux Ubuntu, dentro dele será instalado o Zabbix, todas os templates de banco seram configurados, ficando apenas as configurações de implantação dos servidores.

## Roteiro de criação da imagen.

1 - instalar o docker na maquina:

2 - baixar a imagen do ubuntu:
  ``docker pull ubuntu``
  
3 - Criar o contener
  ``docker run --name zabbix -it ubuntu``

4 - Iniciar o contener
  ``docker start zabbix``

4 - Entra no contener para iniciar a instalação do e configuração do Zabbix.
  ``docker exec -it zabbix /bin/bash``

### Observação: a imagen do ubuntu, vem com varias ferramentas faltando, com isto é preciso instalar elas antes de iniciar a instalação do zabbix.

Instalar ferramenta de IP:
  `` apt-get install iproute2 -y``
Testa a instalação com o commando:
  `` ip a ``

Instalar ferramenta que controla os repositorios do ubuntu:
  ``apt-get install wget -y``
  

  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  


