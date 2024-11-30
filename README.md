# LARAVEL + NGINX + MYSQL
Infraestrutura Docker-compose para criação de ambiente local de desenvolvimento em ecossistema Laravel 11.

- PHP 8.3
- MySQL 8.4.3

# Instruções de uso
- Fazer o download do repositório para Windows WSL / Linux / MacOS (garantir que o Docker está disponível no sistema)
- Dentro da pasta do repositório executar o comando
  > docker-compose up -d
- Vão ser criados 3 containers: laravel_nginx, laravel_php e laravel_mysql
- Utilizar o VSCode para acessar remotamente ao container de php e usar como pasta de trabalho /var/www/html

# Criação de projeto Laravel
- Executar o comando
  ```docker exec -ti laravel_php bash```
