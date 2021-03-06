# LigeroSmart Stack

Configuração básica para instanciar serviços do LigeroSmart

# Pré-requisitos

* arquivos deste repositório
* docker instalado
* docker-compose instalado

# Comandos para iniciar uma instância nova
```
docker-compose up
```
Lembrando que este comando deve ser sempre rodado no diretório onde se encontra o arquivo docker-compose.yml

## Usando make
```
make up
```
Você pode usar ainda outros parâmetros. Consulte o comando `make help`

# Para opção usando Swarm com Proxy Reverso Traefik
```
docker stack deploy -c ligero-swarm.yml ligero
```



# Primeiro acesso

O ambiente será configurado e funcionará na porta 8008

Na primeira execução o sistema é configurado para você. Aguarde até que todas as configurações sejam aplicadas.
A tela de login será carregada automaticamente ao final da configuração.

* Endereço: http://localhost:8008/otrs/index.pl
* Usuário: root@localhost
* Senha: ligero

Informações de acesso do Grafana:
* Endereço: http://localhost:3000
* Usuário: admin
* Senha: ligero

Caso queira acessar remotamente, troque o endereço localhost pelo IP do seu servidor
