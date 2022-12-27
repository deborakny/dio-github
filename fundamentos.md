Git
Sistema de versionamento de arquivos, que permite controlar as modificações feitas neles. 

Github
Plataforma de hospedagem de arquivos que utilizam o git; Trabalha com repositórios, que são como os diretórios, para armazenar os projetos.

Git Bash
Terminal do git, utilizado para inserir os comandos e controlar os repositórios

Secure Hash Algorithm (SHA)
- É um conjunto de funções hash criptográficas 
- A encriptação gera conjunto de characteres identificador de 40 dígitos

Objetos internos:

Blobs:
- blocos básicos de composição
- contém metadados do git
- objetos onde ficam guardados os arquivos
- Possui o tipo (blob), tamanho do arquivo, \0 e o conteúdo
- Guarda o SHA do arquivo

Tree:
- Armazena e aponta para os blobs, commits e outras trees
- Guarda o NOME do arquivo
- Responsável pela estrutura da localização dos arquivos

Commit:
- Aponta para uma tree, parente (último commit realizado antes dele), autor, mensagem e timestamp (hora que foi criado)
- Envia as alterações feitas no projeto

Branch:
- Ramificação do projeto
- Permite a correção de erros e a adição de novos recursos, sem que os arquivos do projeto principal sejam afetados  
- São criadas a partir de uma branch já existente
- Pode ser criada a partir da branch principal
- Pode ser mesclada posteriormente com a branch principal