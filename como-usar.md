# Instruções

## Inicializar um repositório git vazio
Comando: git init

Mandar os arquivos criados ou alterados para a Staging Area (local temporário, onde ficam as mudanças que serão adicionadas)
comando: git add . 

Mandar apenas um arquivo para a staging area
comando: git add nomedoarquivo

Exibir as mudanças que serão "commitadas"
comando: git status

Fazer o commit
comando: git commit -m "título do commit"

(Caso seja necessário alterar a nomenclatura master para main)
comando: git branch -m "main"

- Entrar na conta do Github e acessar o repositório para onde irão os commits
- code > copiar a URL 

Fazer a conexão do repositório local com o repositório remoto 
comando: git remote add origin <colar o link copiado>

Mover os commits do repositório atual para o repositório remoto
comando: git push -u origin main

Para alterar e adicionar arquivos:

comando: git add .
ou
comando: git add nomedoarquivo

comando: git commit -m "Título do commit"

comando: git push -u origin main
OBS.: Não precisa do comando git remote, uma vez que a conexão com o github já está estabelecida

Criar uma branch:

Sair da branch atual (principal) e ir para a que está sendo criada
comando: git checkout -b "nome da branch"

comando: git add .

comando: git commit -m "Título do commit"

comando: git push -u origin nome-da-branch

Para retornar a branch principal
comando: git checkout main
