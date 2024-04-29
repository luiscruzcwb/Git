## Git
Projetos e estudos sobre Git.

![enter image description here](https://www.benner.com.br/tecnologia/wp-content/uploads/2023/10/Git.png)

### **Git** é:
- Controle de Versão
- Armazenamento em Nuvem
- Colaborativo

### Objetos Internos

- Blobs
- Trees
- Commits

### Instalação

**Linux**
- `apt install git`
- `add-apt-repository ppa:git-core/ppa`
- `apt update`
- `apt install git`

### Configurando

**Criando chave SSH**

`ssh-keygen -t ed25519 -C "usuario@email.com"`

**Local de Armazenamento**

`/home/%userhome%/.ssh`

**Corrigir permissões do arquivo**

`chmod 600 /home/%userhome%/.ssh/id_ed25519`

**Copiar a chave Pública**

`cat "nome da chave"`

**Inicializar**

`eval "$(ssh-agent -s)"`

**Enviar a chave**

`ssh-add "nome da chave"`

**Teste copiando um repositório privado**

`git clone git@github.com:luiscruzcwb/luiscruz.com.br.git` # Altere para o seu endereço

### Corrigir Erros

- sudo apt install xdg-utils
- touch ~/.ssh/config
- nano config

### Primeiros Comando / Principais comandos

`git help`

`git init`
- `git config --list`
- `git config --global user.email usuario@email.com`
- `git config --global user.name Nome Sobrenome` **Caso seja preciso atualizar os dados:**
- `git config --global --unset "mudar o que precisa"`

`git add`
- `git add *`
- `git add/rm`

`git commit`
- `git commit -m "Descrição do Commit"`

`git push`
- `git push -v`
- `git push -4`
- `git push -u origin main`
- `git push --force / git push -f`

Adicionar arquivos:
- `git remote add origin https://github.com/%UserName%/%RepositoryName%.git`
- `git remote -v`
- `git branch -M main`

`git status`
- `git status -v`

`git branch "nome"`
- `git branch --all`
- `git checkout "nome da branch"`
- `git push --set-upstream origin "nome da branch"`

`git checkout`
- `git checkout -b`
- `git checkout -f`
- `git checkout --`

### Conflitos ou Erros

- fatal: Authentication Failed
	- `git remote -v`
	- `git remote set-url origin git@github.com:<user>/<repo>.git`
	- `git remote set-url origin git@gitlab.com:<user>/<repo>.git`

### Links 
[Documentação Github](https://docs.github.com/pt/get-started)

[Documentação GIT](https://git-scm.com/doc)

[O que é o Git?](https://learn.microsoft.com/pt-br/devops/develop/git/what-is-git)
