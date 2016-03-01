Padrão para criação da modelagem do Banco de Dados
---------------------------------------------------

Nomenclatura nome base de dados referente a descrição geral do projeto, de preferência uma palavra


Nomenclatura nome tabelas, utilizar inicialmente prefixo de 3 letras, baseado na Descrição do projeto.
Prefixo é definido apartir da primeira letra e as duas letras da última palavra. 
Se existir 3 palavra, pega o primeiro caracter de cada palavra;
Se existir 4 palavra, pega o primeiro caracter da primeira palavra e o primeiro caracter das duas últimas palavras;
Se existir uma palavra a descrição do projeto, pega-se as 3 primeiras letras.
E assim por diante.


Exemplos:

 - Descrição do projeto -> Brasilfone
 	- Prefixos -> bra

 - Descrição do projeto -> Gestão de Cerveja
 	- Prefixos -> gce

 - Descrição do projeto -> Gestão de Pão
	- Prefixos -> gpa

 - Descrição do projeto -> Módulo Financeiro
	- Prefixos -> mfi

 - Descrição do projeto -> Sistema portal bft
	- Prefixos -> spb


Isso se aplica para a nomenclatura da tabela

Exemplos:

Tabela Pessoa:
 - spb_pessoa (inicia com o prefixo definido)

Tabela Pessoa Fisica:
 - spb_pessoa_fisica

Tabela Usuario:
 - spb_usuario

Tabela Historico Operadora:
 - spb_historico_operadora

Tabela Historico Controle Status:
 - spb_historico_controle_status
