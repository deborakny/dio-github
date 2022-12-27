## Chaves SSH:
- Forma de estabelecer uma conexão segura e encriptada entre duas máquinas (no caso, servidor do github e a máquina local)
- Chave pública - será inserida no github, para que ele reconheça a máquina local e a configure como uma máquina confiável

### Como acessar a chave SSH:
:small_orange_diamond: Entrar na conta do github

:small_orange_diamond:Settings

:small_orange_diamond:SSH and GPG Keys

:small_orange_diamond:New SSH Key

:small_orange_diamond:Abrir o Git Bash

:small_blue_diamond:comando: ssh-keygen -t ed25519(criptografia da chave) -C email(preferencialmente o usado no github)

- irá exibir o local onde será armazenada a chave (recomendado)
:small_orange_diamond:Inserir uma senha para a chave

:small_blue_diamond:comando: cd <diretório da chave> 

:small_blue_diamond:comando: cat id_ed25519.pub
- Irá exibir a chave pública

:small_orange_diamond: Copiar

:small_orange_diamond:Voltar ao github

:small_orange_diamond:Title: (Escolher o título)

:small_orange_diamond:key: colar

(ainda no diretório da chave)

:small_blue_diamond:comando: eval $(ssh-agent -s)

:small_blue_diamond:comando: ssh-add id_ed25519 (que é a chave privada)

:small_orange_diamond:Inserir a senha da chave

### Clonar repositório:
:small_orange_diamond:Acessar o repositório a ser clonado

:small_orange_diamond:Code > oferece as URLs para copiar

:small_orange_diamond:Copiar o caminho SSH (não o HTTPS)

:small_blue_diamond:comando: cd <diretório do repositório que será clonado>

:small_blue_diamond:comando: git clone <colar o caminho ssh>
  
- (yes/no/[fingerprint])? yes
  
:small_blue_diamond:comando: ls
  
- exibirá o repositório clonado

**OBS.: A chave pode ser deletada e é possível gerar uma nova, repetindo todo o processo**
