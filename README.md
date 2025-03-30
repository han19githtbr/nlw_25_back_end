## comandos docker

docker-compose build --no-cache connect-node


docker exec -it nlw-connect-node-connect-pg-1 psql -U docker -d postgres

docker compose exec connect-node bash

docker-compose exec connect-node bash -c "npm install && npm run db:migrate"

## executar o ngrok no terminal do back-end

ngrok http http://localhost:3333

## O comando docker-compose up -d é usado para iniciar e executar aplicações de múltiplos contêineres definidas em um arquivo docker-compose.yml. Vamos detalhar cada parte do comando

## acompanhar os logs do frontend em tempo real.

docker-compose logs -f connect-frontend


## acompanhar os logs do back-end em tempo real.

docker-compose logs -f connect-backend


## verificar os logs dos serviços de banco de dados e cache

docker-compose logs -f connect-pg

docker-compose logs -f connect-redis


## reconstruir e iniciar os contêineres com as novas configurações.

docker-compose up -d --build


## Verificar a Rede Docker:

docker network inspect <nome_da_rede>


## rede Docker que os contêineres estão usando

docker network inspect nlw_25_back_end_default