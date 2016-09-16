# Ramificação(branch) no GIT

Lista branch:

- git branch

Cria branch:

- git branch teste

Seleciona o branch:

- git checkout teste

Atalho para os dois comandos acima:

- git checkout -b teste

Voltar pro branch master:

- git checkout master

Deletar branch:

- git branch -d teste

Fazer o merge das alterações(estar no master):

- git merge teste

Criar pelo github um branch chamado develop, onde as funcionalidades que vc está trabalhando sejam comitadas sempre para o develop, e apenas quando a funcionalidade estiver pronta seja feito o merge para o master. Ambientes em produção só deve existir o branch master.


Branch

- master (manter no github e repositório, sempre a versão estável)

- develop (manter no github e não no repositório, sempre a versão em desenvolvimento)

- topic (manter apenas no repositório, são branch pequenos, divididos por funcionalidade)


Obs.: Nunca alterar o branch master, criar branch para nova funcionalidade ou correção para fazer o merge no master, de preferência mudanças pequenas para cada branch. Caso esteja trabalhando em um branch e deseja alterar para outro, faça o commit no branch que você estiver e depois crie um novo branch para trabalhar.
Sempre remova o branch depois de utilizar e não envie para o repositório.

Link documentação: [https://git-scm.com/book/pt-br/v1/Ramifica%C3%A7%C3%A3o-Branching-no-Git](https://git-scm.com/book/pt-br/v1/Ramifica%C3%A7%C3%A3o-Branching-no-Git)

Segue Repósitorio para realizar testes utilizando branch: [https://github.com/Brasilfone/teste-branch.git](https://github.com/Brasilfone/teste-branch.git)

### Início de trabalho com branch

1. Criar o branch **develop** e um branch de **trabalho**

        git branch develop
        git branch trabalho

### Fluxo para subir arquivos para o GIT

1. Commitar os arquivos do branch **trabalho**

        git checkout trabalho
        git add .
        git commit -m "mensagem"

2. Entrar no branch **develop** e fazer o merge com o branch de **trabalho**

        git checkout develop
        git merge trabalho

3. Executar o push no branch **develop**

        git push origin develop

### Fluxo para baixar arquivos do GIT

1. Entrar no branch **develop** e executar o pull

        git checkout develop
        git pull origin develop

2. Entrar no branch de **trabalho** e fazer o merge com o **develop**

        git checkout trabalho
        git merge develop