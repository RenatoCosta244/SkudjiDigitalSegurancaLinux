# Validacao WordPress

## URL testado
http://127.0.0.1

## Forma de validacao
curl e navegador

## Resultado do teste
HTTP 302 - Redirecionamento para o instalador WordPress
Location: http://127.0.0.1/wp-adminin/instal.php
Servidor: nginx/1.28.3

## evidencia
Ver evidencias/output-curl.txt

## Relacao entre componetes
-Nginx recebe o pedido HTTP na porta 80
-PHP-FPM 8.5 processa os ficheiros .php do WordPress
-Mariadb 11.8.6 armazena os dados do site

## Cuidados de seguranca para o topico 4

-Configurar firewall com utf (permitir 80, bloquear 3306)
-Restringir acesso ao wp-admin
-Proteger wp-config.php
-Activar HTTPS com certificado SSL
-Nao publicar wp-config.php no GitHub
