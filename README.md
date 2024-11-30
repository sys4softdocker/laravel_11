# LARAVEL
Infraestrutura Docker-compose para criação de ambiente local de desenvolvimento em ecossistema Laravel 11.

- NginX
- PHP 8.3
- MySQL 8.4.3

# Instruções de uso
- Fazer o download do repositório para Windows WSL / Linux / MacOS (garantir que o Docker está disponível no sistema)
- Dentro da pasta do repositório executar o comando
  > docker-compose up -d
- Vão ser criados 3 containers: laravel_nginx, laravel_php e laravel_mysql
- Utilizar o VSCode para acessar remotamente ao container de php e usar como pasta de trabalho /var/www/html

# Criação de projeto Laravel
- Executar o comando:
  ```docker exec -ti laravel_php bash```
- Dentro da pasta /var/www/html executar o comando: ```composer create-project laravel/laravel .```
- Vai ser criado um projeto Laravel dentro da pasta de trabalho atual.
- No final do processo, executar o comando: ```chmod -R 777 storage``` e o comando ```chmod 777 database/database.sqlite```
  Estes dois comandos vão dar permissão de escrita à pasta ```storage``` e ao ficheiro ```database.sqlite```
