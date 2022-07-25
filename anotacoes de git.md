## Diferença de comando Windows x Linux

| Windows    | Linux            |
|:----------:|:----------------:|
| -cd        | -cd              |
| -dir       | -ls              |
| -mkdir     | mkdir            |
| -del/rmdir | -rm -rf          |
| -cd ..     | -cd ..           |
| -cls       | -clear(Ctrl+L)   |
| -echo      | -echo            |
|            | -sudo(permissão) |

- cd --> navega entre as pastas

- dir --> listar pastas

- mkdir --> cria nova pasta

- del --> deleta arquivos

- rmdir --> releta repositório

- rm -rf(recursive force) --> deleta repositório

- cd .. --> volta uma pasta anterior

- cls/clear --> limpa terminal

- (tab) --> autocompleta

## Como gerar chave SSH

1. Entrar no terminal git bash

2. digitar comando `ssh-keygen -t ed25519 -C (_email do github_)`

3. colar chave no github

4. para funcionar deve entrar de novo no terminal

5. digitar comando `eval $(ssh-agent -s)`

6. por fim digite comando `ssh-add (_chave_)`

## Inicializando Git

inicializar o repositório do git -->` git init`

mover arquivos, começar versionamento --> `git add`

criar commit -->` git commit`

`ls -a` --> flag que mostra todo arquivo, mesmos os ocultos

comandos (configuração inicial): `git config --global user.email "(_email_)"`

                    `git config --global user.name (_nome_)`

comando `git status`: descreve o status dos arquivos

comando `mv (_nome do arquivo_) ./(_nome da pasta_)`: move arquivo para outra pasta

comando `git add .` ; `git add (_nome do arquivo_)`; `git add *`: move todo arquivo no "staged"

## Trabalhando com github

- _como verificar se as configurações são iguais no github e git_:
  
  comando `git config --list`: lista de todas configuraçõesdo git 
  
  tecla "q" para sair

- _como mudar configuração do git_:
  
  - comando `git config --global --unset (propriedade específica da configuração)`
  
  - reusar comandos (configuração inicial)

- _como por repositório local para remoto(github)_:
  
  - comando `git remote add origin(apelido) (_link do github_)`
  
  - comando `git remote -v`: lista as listas de repositório remoto
  
  - comando `git push origin master(branch)`: sobre conteúdo no repositório

- comando `git pull origin master`: puxa conteúdos do repositório
