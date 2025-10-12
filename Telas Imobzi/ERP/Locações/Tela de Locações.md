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
- **[[Tela de Imóveis|Imóvel]]**: Imóvel que será locado. Pode ser filtrado com o [[Filtro do Imóvel|filtro de imóvel]] ao adicioná-lo clicando no ícone de filtro;
- **[[Tela de Contatos|Locatários]]**: Os contatos que serão locatários dessa locação. Caso tenha mais de um locatário, poderá selecionar qual deles será o pagador;
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
- **[[Garantia|Garantia]]**;
- **Seguros e adicionais**: Para adição do seguro do imóvel ou seguro incêndio;
- **Itens da fatura de aluguel**: Seção para inserção de valores a serem cobrados por cima do aluguel;
	- **Descrição**: O nome ou descrição do item;
	- **Valor**: Quanto será cobrado deste item;
	- **[[Comporatamento do Item da Locação|Comportamento]]**;
	- **[[Tela de Contatos|Fornecedor]]**: O fornecedor da despesa. No caso do IPTU, é a prefeitura da cidade;
	- **Pagar automaticamente no vencimento**: Caso a despesa será paga automaticamente no dia do vencimento;
		- **Método de pagamento da despesa**.
	- **Recorrente**: Marque caso esse item será cobrado mais de uma vez;
		- **Quantidade de parcelas**: Quantas vezes o item ocorrerá. Caso o item for ser cobrado por tempo indeterminado, mesmo após o término da locação, insira "999" neste campo;
		- **Parcela atual**: A quantidade de parcelas já pagas;
	- **Calcular o IRRF e incluir na DIMOB**: Apenas deve ser marcado como itens que serão considerados renda para o proprietário, como multas. Para as despesas do imóvel como IPTU, Condomínio, obra e outros, não será necessário. Caso o IRRF seja recolhido a maior ou menor, não há motivo para preocupações, já que na 'Declaração de Imposto de Renda', a Receita Federal calculará o valor total a ser pago no ano, descontando o que foi recolhido, dando um valor a pagar ou a restituir para o proprietário.
	- **Descontar taxa de administração**: Caso desse item será descontada a taxa de administração da imobiliária;
	- **Lançar o item a partir de uma data**: Para caso o item só passará a ser lançado a partir de uma data específica.
		- **Data de início**;
	- **Editar referência da fatura**;
		- **Data de início, Data de término e Data de vencimento da próxima fatura**: Usado para alterar a referência da fatura da locação a partir de uma data de início e uma de fim. O vencimento, caso seja atualizado com uma data não compatível com a que está no campo de "Dia do vencimento" da locação na primeira página do menu, irá ser trocado pelo novo valor inserido.
- **Configurações de cobrança**;
	- **Meio de recebimento**: Você pode configurar qual conta bancária será exibida na fatura para que o locatário possa realizar a transferência. Para isso, acesse no Imobzi o menu Administrador > Ícone da locação e preencha os dados da sua conta bancária no campo Dados para transferência;
		- **Cartão, boleto e pix**: Os três métodos ficam disponíveis, facilitando o pagamento. Para que funcionem corretamente, é necessário que a integração com o PJBank esteja ativa. Caso necessite que o QR code seja gerado junto ao boleto, será necessário abrir um chamado com o PJBank para solicitar essa mudança;
		- **Boleto bancário**: A fatura será gerada automaticamente e registrada no PJBank, com a possibilidade de repasse automático em D+2.
		- **Dinheiro**: A fatura também será gerada automaticamente, com a informação "A fatura será paga através de dinheiro". Nesse caso, será necessário realizar a baixa manual da fatura e o repasse ao locador também de forma manual.
		- **Cartão de crédito**: Quando essa opção estiver ativa, o pagamento poderá ser feito apenas com o cartão cadastrado pelo cliente (locatário). Também é possível optar pelo parcelamento, limitado à quantidade de parcelas liberada na locação;
		- **Transferência**: A fatura será gerada automaticamente, com a informação "A fatura será paga através de transferência". Assim como no pagamento em dinheiro, será necessário fazer a baixa manual da fatura e o repasse ao locador manualmente.
		- **Pix**: A fatura será pagável apenas através de pix.
	- **Cobrar multa após vencimento e Cobrar juros de mora após vencimento**: Ativáveis caso se deseje cobrar uma multa ou juros por dia após a data de vencimento da fatura. Cobrados acima do valor da fatura, não do aluguel. Os padrões podem ser alterados dentro de Administrador > Locação;
	- **Calcular IRRF automaticamente**: Ao selecionar essa opção o imposto de renda desta locação será retido na fonte e pode-se emitir um informe de rendimentos na aba de Receita federal do Imobzi. Conforme a Lei nº 14.663, de 28/08/2023, o cálculo do IRRF é obrigatório quando o Proprietário for Pessoa Física e o Inquilino Pessoa Jurídica. Por padrão, o Imobzi aplicará também o Desconto Simplificado da referida lei. ATENÇÃO: Não será calculado o IRRF, caso o valor seja igual ou inferior a R$10,00, conforme artigo 67 da Lei nº 9.430/1996.
	- **Deduzir da base de calculo do IRRF a Taxa de administração**: Ao selecionar essa opção, o IRRF será calculado levando em consideração a taxa de administração da locação. Caso não selecione, o IRRF será sobre o valor bruto do aluguel;
	- **Gerar nota fiscal automaticamente**: Ao selecionar essa opção podemos gerar a nota fiscal da taxa de administração da locação, lembrando que é necessário configurar a integração com o [eNotas](https://help.imobzi.com/pt-br/article/como-gerar-a-nota-fiscal-de-forma-automatica-10sbeos/);
	- **Incluir na DIMOB automaticamente**: Selecione esta opção essa locação será incluída para geração de um relatório da [Dimob](https://help.imobzi.com/pt-br/article/o-que-e-a-dimob-e-como-exporta-la-578vzn/).
- **Taxas de administração**: Defina o 'Tipo de Administração', as taxas que serão cobradas do Proprietário e se o repasse será automático ou manual. Para 'Imóvel próprio' não há taxas.
	- **Tipo de administração**;
		- **Locação administrada pela imobiliária**: