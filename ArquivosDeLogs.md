Padrão para criação de arquivos de logs
---------------------------------------


###Local

Local para os arquivos de logs é /var/log/, seguido do nome do projeto

Exemplos:

 - /var/log/projeto1/
 - /var/log/projeto2/

Dentro do diretórios ficam todos os logs do projeto em questão.


###Nomenclatura arquivo log

O nome do arquivos de log passa pela descrição do que o processo faz, separado por _ cada palavra com extenção .log

Exemplos:

 - /var/log/projeto1/atualiza_status_tabela.log
 - /var/log/projeto1/cria_tabelas_mensais.log


###Padrão registros de log nos arquivos

O conteúdo no arquivo de log é sempre separado por uma linha em branco para cada interação, se o script roda a cada 30 minutos, cada novo log dos 30 minutos é separado por uma linha em branco.

Cada log mantém essa estrutura:

[data e hora] [descrição] [status]

[data e hora] [descrição] [status]

[data e hora] [descrição] [status]


Exemplos:

23/03/2016 17:23:16 CONNECT base1 OK

23/03/2016 17:23:46 CONNECT base2 ERRO: mensagem de erro

23/03/2016 17:24:16 CONNECT base1 OK
