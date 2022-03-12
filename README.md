
# Stack EFK (Elasticsearch, Fluentd, Kibana)

#### Requisitos

* Docker 
* Docker Compose

## Criar a network abaixo antes de dar start

```shell
docker network create --attachable --subnet 10.0.1.0/24 backend
```

#### Os arquivos de LOG devem ser colocados na pasta `fluentd/logs`

#### Executar o comando abaixo para subir a Stack EFK

```shell
docker-compose up -d --build
```
#### Executar o comando abaixo para verificar se o Fluentd está fazendo parse corretamente olhando seu LOGS

```shell
docker logs fluentd_fluentd_1 -f  
```
