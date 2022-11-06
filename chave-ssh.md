Chaves SSH:
- Forma de estabelecer uma conexão segura e encriptada entre duas máquinas (no caso, servidor do github e a máquina local)
- Chave pública - será inserida no github, para que ele reconheça a máquina local e a configure como uma máquina confiável

Como acessar a chave SSH:
- Entrar na conta do github
- Settings
- SSH and GPG Keys
- New SSH Key

- Abrir o Git Bash
comando:
ssh-keygen -t ed25519(criptografia da chave) -C email(preferencialmente o usado no github)

- irá exibir o local onde será armazenada a chave (recomendado)
- Inserir uma senha para a chave

comando: cd <diretório da chave> 
comando: cat id_ed25519.pub
- Irá exibir a chave pública
- copiar
- Voltar ao github
- Title: (Escolher o título)
- key: colar

(ainda no diretório da chave)
comando: eval $(ssh-agent -s)
comando: ssh-add id_ed25519 (que é a chave privada)
- inserir a senha da chave

Clonar repositório:
- Acessar o repositório a ser clonado
- Code > oferece as URLs para copiar
- Copiar o caminho SSH (não o HTTPS)

comando: cd <diretório do repositório que será clonado>
comando: git clone <colar o caminho ssh>
(yes/no/[fingerprint])? yes
comando: ls
- exibirá o repositório clonado

OBS.: A chave pode ser deletada e é possível gerar uma nova, repetindo todo o processo