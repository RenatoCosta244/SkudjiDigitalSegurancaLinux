# publicacao Wordpress

## Nivel escolhido
Nivvel 3 - Avancado

## Rota escolhido
Nginx

## Componentes usados

-Servidor web: Nginx 1.28.3
-PHP: PHP 8.5-FPM
-Base de dados: MariaDB 11.8.6
-WordPress: versao oficial wordpress.org

## Pasta de publicacao
/var/www/html/wordpress

## Estado da instalacao

Intalador acessivel - HTTP 302 redirect para wp-admin/install.php

## Comandos principais utilizados
Sudo apt install nginx -y
sudo apt install php php-fpm php-mysql php-xml php-curl php-gd php-mbstring php-zip
sudo apt install mariadb-server -y
wget https://wordpress.org/latest.tar.gz
tar -xzvf latest.tar.gz
sudo cp -r wordpress/* /var/www/html/wordpress/
sudo chown -R www-data:www-data /var/www/html/wordpress
sudo chown -R 755 /var/www/html/wordpress
sudo ln -s /etc/nginx/sites-available/wordpress /etc/nginx/sites-enabled/
sudo systemctl reload nginx

## limitacoes
-Repositorio cdrom causava erro no apt update - resolvido removendo cddrom.sources
-Ficheiro latest.tar.gz teve ser descaregado duas vezes
-VM em modo NAT nao permitia acesso externo - resolvido mudando para Bridge
