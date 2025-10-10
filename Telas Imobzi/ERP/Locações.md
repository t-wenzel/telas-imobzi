---
tags:
FAQs Relacionadas:
---
---
## Definição

Nesta tela geram-se e gerenciam-se os contratos de aluguel. O usuário pode criar novas locações vinculando imóvel, proprietário, inquilino e valores, e definir ciclos de cobrança (mensal, trimestral etc.). Há funcionalidade de reajuste automático de aluguéis e contratação de seguros (por exemplo, Seguro Incêndio pela Migra Seguros) diretamente nesta ficha. Também aqui se emitem as faturas mensais automaticamente. Locações consolida o ciclo de vida dos contratos de aluguel;

## Campos de Nova Locação e Edição de Locação

- **Termos da locação**;
	- **Tipo da Locação**: Para o tipo de locação;
		- **Residencial**;
		- **Não residencial**;
		- **Comercial**;
		- **Industrial**;
		- **Self storage**;
		- **Temporada**.
	- **Status**: Status inicial da locação;
		- **Ativo**;
		- **Encerrado**;
		- **Em progresso**;
		- **Suspenso**.
		- **Rescindida**: Apenas após criar a locação fica disponível, e poderá ser aplicado para esses casos.
	- **Categoria**: Para alterar as tags das faturas automáticas nas locações;
	- **Data de início, data de término e duração do contrato**: Onde são colocadas as datas referentes à locação e quanto tempo ela durará;
	- **Contrato por tempo indeterminado**: Ative caso a locação irá continuar gerando faturas mesmo após seu termino;
- **Imóvel**: Imóvel que será locado. Pode ser filtrado com o [[Filtro do Imóvel|filtro de imóvel]] ao adicioná-lo clicando no ícone de filtro;
- **Locatários**: Os locatários dessa locação. Caso tenha mais de um locatário, poderá selecionar qual deles será o pagador;
- **Definição de valores**
	- **Valor da locação**: Valor do aluguel dessa locação.
	- **Modo de cobrança**;
		- **Normal**: Padrão do pagamento de aluguel;
		- **Aluguel antecipado**: O inquilino antes paga o valor do aluguel, para depois residir nele;
	- **Dia de vencimento**: O dia do mês em que a fatura da locação irá vencer (podendo também ser no último dia do mês);
	- **Índice de reajuste**: O índice que definirá o reajuste do valor da locação a cada doze meses;
	- **Cobrar proporcional junto ao 2º aluguel**: Para caso se queira atrasar a cobrança do primeiro aluguel para ser junto à 2ª cobrança, com o valor proporcional à referência da locação;
	- **Este contrato já está em andamento**: Para, caso o contrato de locação já esteja ocorrendo quando ele foi criado na Imobzi, o reajuste ocorrer na data correta. Ao gerar a primeira fatura o Imobzi marcará essa opção automaticamente e não será possível mudá-la.;
		- **Data do último reajuste**: Quando o último reajuste do aluguel ocorreu. Se inserida uma data retroativa com mais de 12 meses, o Imobzi realizará automaticamente o reajuste no dia seguinte de forma automática, porque considera que não houve reajuste no último ano;
		- **Valor original do contrato**: Valor informativo sobre o qual será calculado o primeiro reajuste.
	- **Garantia**: