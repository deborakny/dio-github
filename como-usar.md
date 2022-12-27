# Instruções

### Inicializar um repositório git vazio
:small_blue_diamond:Comando: git init

### Mandar os arquivos para a Staging Area 
(local temporário, onde ficam as mudanças que serão adicionadas)

:small_blue_diamond:comando: git add . 

### Mandar apenas um arquivo para a staging area
:small_blue_diamond:comando: git add nomedoarquivo

### Exibir as mudanças que serão "commitadas"
:small_blue_diamond:comando: git status

### Fazer o commit
:small_blue_diamond:comando: git commit -m "título do commit"

(Caso seja necessário alterar a nomenclatura master para main)

:small_blue_diamond:comando: git branch -m "main"

:small_orange_diamond: **Entrar na conta do Github e acessar o repositório para onde irão os commits**

:small_orange_diamond: **code > copiar a URL**

### Fazer a conexão do repositório local com o repositório remoto 
:small_blue_diamond:comando: git remote add origin <colar o link copiado>

### Mover os commits do repositório atual para o repositório remoto
:small_blue_diamond:comando: git push -u origin main

### Para alterar e adicionar arquivos

:small_blue_diamond:comando: git add . ou :small_blue_diamond:comando: git add nomedoarquivo

:small_blue_diamond:comando: git commit -m "Título do commit"

:small_blue_diamond:comando: git push -u origin main
  
OBS.: Não precisa do comando git remote, uma vez que a conexão com o github já está estabelecida

### Criar uma branch

:small_orange_diamond:**Sair da branch atual (principal) e ir para a que está sendo criada**
  
:small_blue_diamond:comando: git checkout -b "nome da branch"

:small_blue_diamond:comando: git add .

:small_blue_diamond:comando: git commit -m "Título do commit"

:small_blue_diamond:comando: git push -u origin nome-da-branch

### Retornar a branch principal
:small_blue_diamond:comando: git checkout main
