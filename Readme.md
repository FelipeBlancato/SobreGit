# Instruções sobre Git e Versionamento

# 1 - Git Bash:
### Comandos Básicos:
git --version (-v) || Verificar versão do software  
git init || Cria um repositório local vazio no diretório atual   
git add || Adiciona arquivos ao Staging  
(add . para todos os arquivos)  

### Configuração GitHub:
git remote add origin *link do rep* || Linka os dois repositórios, "origin" é o nome  
(SSH exige configuração mas evita autenticações)    
ssh-keygen -t ed25519 -C "e-mail" || Gera uma chave SSH  
(Copiar a chave id.pub e colar no GitHub)  

### Comandos Commit:
git status || Ver status do processo  
git commit || Fazer um commit do Staging (-m ou --message para adicionar nota)  
git log || Lista os commits (aperte Q para sair)  
git push -u origin main || Envia os arquivos no repositório git para o github  
(-u é abreviação de --set-upstream, as próximas linhas podem usar apenas "push")  

### Comandos Branch:
git branch "nome" || Cria uma nova branch  
git checkout || Muda de branch  
git checkout -b || cria e muda  
git branch -M "" || renomeia a branch  
(-M equivale ao --move + --force) 

### Projetos Compartilhados:
git clone || Cria um repositório local de um projeto no GitHub  
git pull || Atualiza o diretório local com os commits do GitHub  

# 2 - Linha de Comando:
### Configuração Git:
sudo apt update || Atualiza a lista de pacotes  
sudo apt upgrade || Atualiza pacotes já existentes  
sudo add-apt-repository ppa:git-core/ppa || Adiciona o repositório do Git à lista  
sudo apt update  
sudo apt install git  

git config --global user.name "Your Name"  
git config --global user.email yourname@example.com  
git config --get user.name  
git config --get user.email  

git config --global init.defaultBranch main || Troca o nome da branch  
git config --global pull.rebase false || Mantém merge ao invés de rebase  

ls ~/.ssh/id_ed25519.pub  
ssh-keygen -t ed25519  
cat ~/.ssh/id_ed25519.pub  

git clone git@github.com:USER-NAME/REPOSITORY-NAME.git || Quando o rep foi criado primeiro no Github, podemos clonar ao invés de apenas linkar com o "remote add"  