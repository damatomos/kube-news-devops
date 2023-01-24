# Projeto kube-news

### Objetivo
O projeto Kube-news é uma aplicação escrita em NodeJS e tem como objetivo ser uma aplicação de exemplo pra trabalhar com o uso de containers.

### Configuração
Pra configurar a aplicação, é preciso ter um banco de dados Postgre e pra definir o acesso ao banco, configure as variáveis de ambiente abaixo:

DB_DATABASE => Nome do banco de dados que vai ser usado.

DB_USERNAME => Usuário do banco de dados.

DB_PASSWORD => Senha do usuário do banco de dados.

DB_HOST => Endereço do banco de dados.

### Imagem docker

Para rodar a imagem docker

```
cd ./src
docker container run -d --rm -p 8080:8080 damatomos/kube-news
```

### Kubernetes

Para rodar o kubernetes

```
cd ./k8s
kubectl apply -f deployment.yaml
```
