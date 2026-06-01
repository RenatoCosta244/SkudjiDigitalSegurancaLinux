# Topico 1 - Preparacao ao ambiente linux

## Ambiente utilizado
VM local 

## Objectivo desta actividade
Preparar o ambiente Linux e organizar as primeiras  evidencias tecnicas

## Estrutura criadas
->pasta principal linux-seguranca-cloud
  ->pasta topico-01
    -> pasta evidencias
    -> comandos-topico-01.txt
    ->README.md
  ->pasta projecto-final

## Comandos executados
mkdir -Criacao de pastas
ls -l -Printa os dados encontrados no directorio
touch -Cria tipos de ficheiros
cd nomepasta -Entra em uma pasta com o nome da pasta
sudo apt update && sudo apt upgrade -y -Atualizacao do sistema linux
sudo ufw enable  -Configura o firewall	
nano README.md  -Cria um ficheiro raedme.md
sudo systemctl status ssh
cat README.md
ip a

## Diferenca entre VM, VPS e infrastrutura em nuvem
VM E uma maquina virtual, e uma maquina dentro da sua maquina local
VPS E um servidor da sua empreca onde podes acessar atraves do computador
infrastrutura em nuvem sao conjuntos de servicos prestados aos clientes como armazenamentos, servidores, base de dados.

## Dificuldades encontradas
Tive que activar a virtualizacao no bios
Aumento de armazenamento do linux


## Proximos passos 
Configurar o firewall
Configurar o SSH para ter acesso atraves do windows.
