Ramificação(branch) no GIT
==========================

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

Obs.: Nunca alterar o branch master, criar branch para nova funcionalidade ou correção para fazer o merge no master, de preferência mudanças pequenas para cada branch. Caso esteja trabalhando em um branch e deseja alterar para outro, faça o commit no branch que você estiver e depois crie um novo branch para trabalhar.
Sempre remova o branch depois de utilizar e não envie para o repositório.

Link documentação: [https://git-scm.com/book/pt-br/v1/Ramifica%C3%A7%C3%A3o-Branching-no-Git](https://git-scm.com/book/pt-br/v1/Ramifica%C3%A7%C3%A3o-Branching-no-Git)

Segue Repósitorio para realizar testes utilizando branch: [https://github.com/Brasilfone/teste-branch.git](https://github.com/Brasilfone/teste-branch.git)