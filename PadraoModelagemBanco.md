Padrão para criação da modelagem do Banco de Dados
---------------------------------------------------

Nomenclatura nome base de dados:
 referente a descrição geral do projeto, de preferência uma palavra


###Nomenclatura nome de tabelas:

Utilizar inicialmente prefixo de 3 letras, baseado na Descrição do projeto.
Se existir 1 palavra, pega-se as 3 primeiras letras;
Se existir 2 palavras, pega a primeira letra da primeira palavra e as duas primeiras letras da última palavra;
Se existir 3 palavras, pega a primeira letra de cada palavra;
Se existir 4 palavras ou mais, pega a primeira letra da primeira palavra e a primeira letra das duas últimas palavras;


Exemplos:

 - Descrição do projeto -> Brasilfone
 	- Prefixo -> bra

 - Descrição do projeto -> Gestão de Cerveja
 	- Prefixos -> gce

 - Descrição do projeto -> Gestão de Pão
	- Prefixo -> gpa

 - Descrição do projeto -> Módulo Financeiro
	- Prefixo -> mfi

 - Descrição do projeto -> Sistema portal bft
	- Prefixo -> spb


Isso se aplica para a nomenclatura das tabelas


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


###Nomenclatura campos das tabelas:

Exemplos:

Tabela spb_pessoa:
 - pes_id PK
 - pes_nome
 - pes_data_cadastro

Tabela spb_pessoa_fisica:
 - pfi_id PK
 - pfi_pes_id FK
 - pfi_cpf
 - pfi_rg

Tabela spb_historico_controle_status:
 - hcs_id PK
 - hcs_status
 - hcs_data_atualizacao

Tabela spb_historico_sms_processando_operadora:
 - hpo_id PK
 - hpo_total
 - hpo_data


###Nomenclatura para chaves estrageiras:

Exemplos:

Tabela spb_pessoa com a tabela spb_pessoa_fisica:
 - pes_id PK
 - pes_nome
 - pes_data_cadastro
 - pes_pessoa_fisica

Tabela spb_pessoa_fisica com a tabela spb_historico_controle_status:
 - pfi_id PK
 - pfi_cpf
 - pfi_rg
 - pfi_historico_controle_status
