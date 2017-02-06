__Arquivo descritivo sobre o padrão de marcação para liberação de versão:__

A única regra é sobre a tag h1(# PERFIL #) ou (# PERFIL 1, PERFIL 2#) demarca o perfil para o qual as alterações tem efeito, o texto deve conter no mínimo 1 perfil, utilizar as tags hN sómente para o demarcar o perfil;

Utilizar o markdown para formatar o testo conforme o exemplo.

__Exemplo de texto:__
 
# Administrativo #
 
__Correções na tela Administrativo > Clientes:__
+ Corrigido bug que fazia com que a grid de clientes recarregasse infinitamente;
+ Corrigido bug que não permitia altualizar os dados do cliente;
+ Adicionados novos campos no cadastro tipo de cliente e incrição municipal;
 
__Melhorias na tela SMS > Clientes:__
+ Agora salva os dados em banco antes de enviar para o sistema de SMS via API;
 
# Customer, Financial #
 
__Melhorias na tela Administrativo > Relatórios > SMS/MT:__
+ No filtro por cliente agora é possvel filtrar pelo digitando o nome do cliente;
+ Adicionado filtro por data e hora do envio de SMS inicial e final;

__Nova funcionalidade tela Administrativo > Contratos pendentes:__
+ Na tela de contratos pendentes aparecem apenas o contratos não fechados com o cliente, nesta tela é possível atualizar os dados do cliente e também fechar os contratos;
 
 
