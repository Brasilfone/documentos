Liberações de Versões
---------------------

- x.x.X Correções de bugs
- x.X.x Melhorias e evoluções
- X.x.x Novas funcionalidades


Utilização das TAGs Git
-----------------------

- git tag (lista tags existente)
- git tag -a v1.0.0 -m "Descrição da versão 1.0.0, principais funcionalidades"
- git tag -d v1.0.0 (remover tag)


Para liberação push no master e na tag, exemplo:

- git push origin master
- git push origin v1.0.0
- git push origin --tags (manda todas as tags)
- git pull origin --tags (baixa todas as tags)


Mudar de versão em produção:

- git checkout v1.0.0 (tirar a utilização do branch master e mudar pra versão v1.0.0)
- git checkout master (voltar pra branch master de desenvolvimento)


Adicionar tag para liberações no ambiente de produção
