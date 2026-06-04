# Permissoes aplicadas

## Ambiente utilizado
   -> VM Local servidor linux ubunto
 
## Utilizador e grupos
   whoami -> renato244costa
   id  -> uid =1000 (renato244costa)   gid =1000(renato244costa)  groups =1000(renato244costa)  27 (sudo)
   grous -> renato244costa sudo

## Ficheiros criados
     -> public.txt
     -> restrito.txt
     -> script.sh

## Permissoes aplicadas
  |  Ficheiro | Permissao | Justificacao |

  | public.txt | 644       | a tudos os users|
   
  | restrito.txt | 640     | dados restritos para utilizadores especificos|
  
  | script.sh   | u + x    | funcoes automatico sao para dono |


## Relacao com principios do menor aplicada
No pubicos sao dados que podem ser partilhadas a todos como o nome dis ou publico mais com  o dono  ler e escrever
grupos so ler e outros so ler

enquanto que restrito sao dados restritos sao para utilizadores restritos ou especificos
dono ler e escrever grupo so ler outros nao tem acesso nenhum

script ja e mais para administradores, sao funcoes automaticos para realizacao de uma tarefa
dono(user) adicionar execucao
