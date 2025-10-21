# Instruções sobre Git e Versionamento
### Download do Git no Site Oficial

## Comandos Básicos:

git --version (-v) || Verificar versão do software  
git init || Cria um repositório vazio no diretório atual   
git add || Adiciona arquivos do diretório ao Staging  
(add . para todos os arquivos)  

## Comandos Commit:

git status || Ver status do processo  
git commit || Fazer um commit do Staging ( -m ou --message para adicionar nota)  
git log || Lista os commits (aperte Q para sair)  

## Comandos Branch:

git branch "nome" || Cria uma nova branch  
git checkout || Muda de branch  
git checkout -b || cria e muda  
git branch -M "" || renomeia a branch  
(-M equivale ao --move + --force) 

## Configuração GitHub:

git remote add origin *link do rep* || Linka os dois repositórios !origin é o nome  
(SSH exige configuração mas evita autenticações)  
(Para colar o link use SHIFT + Insert)  
git push -u origin main || Envia os arquivos no repositório git para o github  
(-u é abreviação de --set-upstream, as próximas linhas podem usar apenas "push")  

## Configuração SSH:

## Para projetos Compartilhados:

git clone || Cria um repositório local de um projeto no GitHub  