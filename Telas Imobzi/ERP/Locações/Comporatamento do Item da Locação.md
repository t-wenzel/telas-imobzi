---
tags:
FAQs Relacionadas:
---
---
## Descrição

Os comportamentos são a maneira que os itens da fatura serão cobrados, repassados, administrados os descontados.

## Campos

- **Cobrar do locatário:** o valor inserido no item será cobrado apenas do locatário, sem vínculo com o repasse e sem ser considerado uma despesa administrada. O saldo cobrado será destinado ao caixa da imobiliária.
- **Cobrar do locatário e administrar pela imobiliária:** ao selecionar este comportamento, o valor do item será cobrado na fatura e também será criado um lançamento correspondente na aba de Lançamentos do Imobzi (fluxo de caixa). É necessário informar a data de vencimento da despesa e o fornecedor — por exemplo, no caso do IPTU, a prefeitura da sua cidade. Lembre-se de cadastrar o fornecedor na tela de Contatos do Imobzi. Se você estiver com a integração do PJBank ativa, também é possível selecionar a opção "pagar automaticamente no vencimento", permitindo a inclusão do código de barras do boleto para pagamento automático. O valor deste item aparecerá como negativo no repasse, na conta do locador, permitindo que ele visualize no recibo que essa despesa foi paga.
- **Cobrar do locatário e repassar para o locador:** ao selecionar este comportamento, o valor do item será cobrado na fatura e somado ao valor do repasse para o locador.
- **Creditar o locatário:** ao selecionar este comportamento, o valor do item será descontado da fatura, mas não será descontado no repasse. Isso significa que a imobiliária deverá ter esse valor em caixa para realizar o repasse integral ao locador.
- **Creditar o locatário e descontar do locador:** ao selecionar este comportamento, o valor do item será descontado da fatura do locatário e o mesmo valor será descontado no repasse da conta do locador.
- **Descontar do Locador:** Com esse novo comportamento, o valor é descontado direto no repasse ao proprietário, sem aparecer na fatura do inquilino e sem alterar o valor total a ser pago. Esse desconto será exibido como “Descontos locador” nos detalhes da fatura. Ideal para manutenções, taxas extras ou qualquer ajuste que precise ser repassado diretamente ao locador.
- **Cobrar do Locador e Administrar pela Imobiliária**: Essa opção também faz a cobrança direto do locador, sem impactar a fatura do inquilino. A diferença é que o item será administrado pela imobiliária, ficando visível apenas na conta do locador.

## Tabela de Comportamentos

|Comportamento|Quem paga|Para onde vai o dinheiro|Papel da imobiliária|Quando usar (exemplos)|
|---|---|---|---|---|
|**Cobrar do locatário**|Locatário|Imobiliária (fica no caixa)|Beneficiária|Multa por atraso, taxa administrativa|
|**Cobrar do locatário e administrar pela imobiliária**|Locatário|Fornecedor (pago pela imobiliária)|Intermediária (entra e sai)|IPTU, condomínio, seguro|
|**Cobrar do locatário e repassar para o locador**|Locatário|Locador|Intermediária|Taxas que o proprietário deve receber além do aluguel (ex.: rateio de despesas reembolsáveis)|
|**Creditar o locatário**|Imobiliária (dá o desconto)|Locador (recebe integral)|Beneficiária negativa (precisa bancar a diferença)|Desconto que a imobiliária decidiu dar ao inquilino sem impactar o repasse do proprietário|
|**Creditar o locatário e descontar do locador**|Locador (indiretamente)|Menor repasse ao locador|Intermediária|Desconto que será dado ao inquilino, mas retirado do valor do proprietário|
|**Descontar do locador**|Locador|Imobiliária (ou fornecedor)|Intermediária|Manutenção, taxas extras ou ajustes pagos direto pelo proprietário|
|**Cobrar do locador e administrar pela imobiliária**|Locador|Fornecedor (pago pela imobiliária)|Intermediária (entra e sai)|Contas do imóvel que o proprietário decidiu que ele mesmo paga, mas a imobiliária administra (ex.: reforma, seguro do imóvel)|