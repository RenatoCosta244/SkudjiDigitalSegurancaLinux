
# Acesso remoto por SSH
  Atraves do powershell abrir como administrador

## O que e SSH?
  SSH e um protucolo que permiti aceder e controlar um computador remotamente de forma
segura atraves da rede, ou mais simples uzar um terminal de outro computador, mas a distancia
tudo o que e escrito vai encriptado pela rede.
ssh renato@ip
ssh protocolo
renato utilizador
ip endereco ip do servidor
O que podemos fazer via ssh
    ->gerir ficheiros e pastas
    ->instalar programas 
    ->ver logs
    ->reiniciar servicos
    ->transferir ficheiros(com scp ou sftp)

tem dois tipos de autenticacao
    ->password 
    ->chave SSH

## Que informacao seria necessaria para aceder a um servidor por SSH?
  Utilizador: renato244
  Endereco IP:
  Porta: normal 2222
  palavra passe: ###############

## Limitacoes encontradas
 Sem limitasoes mais sim dificuldades mais foram ultrapassadas

## Estadp do servidor sudo
sudo apt systemctl openssh-server -y
sudo systemctl restart ssh
sudo systemctl start SSH
sudo systemctl status SSH

# Acesso remoto em chaves SSH

## Diferenca entre autenticacao por palavra-passe e autenticacao por chave
Para utilizares o password utilizas um comando depos se o comando estiver corecto e
pedido o password->  ssh renato@ip, e simples mas menos seguro.
Enquanto que em um par de chaves temos a chave privada(fica no seu computador) e a chave publico(fica no servidor)
Primeiro tem que gerar a par de chave no seu computador
  ->ssh-keygen -t apt25519
Segundo enviar a chave publica para o servidor
  ->ssh-copy-id renato@ip
Terceiro ligar sem password
  ->ssh renato@ip

## Chave publica
Ela e cadeado podes dar a toda a gente, fica no servidor e podes partilhar
## Chave privada
Ela e chave do cadeado (so tu tens), acesso total ao servidor, nao podes partilhar
## Cuidados de seguranca 
Em producao e dizativada o password sao utilizadas as chaves por ser mais seguro
