<!-- TITLE: Integração Bancária Receber (COBRANÇA)-->
<!-- SUBTITLE: Integração Bancária a Pagar -->

1. Introdução
1. Origem
	1. Automática
	2. Manual
2. Processamento
	1. Gerar Boleto
	2. Gerar Arquivo
3. Saida
	1. Boleto
	2. Arquivo
# Introdução
A integração bancária tem a finalidade de integrar a parte finaceiro do sistema com o banco atraves de arquivo de remessa e retorno.

Operacionalmente o usuário gera um arquivo de remessa atraves do sistema, processa esse arquivo no site/aplicação do banco que devolve um arquivo de retorno para o usuário contendo o resultado do processamento. O usuário processa o arquivo no sistema que dependendo da ocorrencia lançada pelo banco executa a baixa ou não do(s) titulo(s).

![Remessa Retorno](/uploads/remessa-retorno.png "Remessa Retorno")

Os títulos podem ter origem pelo processo automático de faturamento de movimentos ou lançados manualmente pelo usuário.

# Origem
## Gerar Fatura
O cliente fatura os fretes gravados no sistema e gerando um título, imprime o boleto para enviar ao seu cliente e gera o arquivo de remessa para processar no banco.

#### Minutas geradas no sistema

![Minuta Gerada](/uploads/minuta-gerada.jpg "Minuta Gerada") ![Minuta Gerada 01](/uploads/minuta-gerada-01.jpg "Minuta Gerada 01")

![Minutas](/uploads/minutas.jpg "Minutas")

	Faturamento
![Faturamento](/uploads/faturamento.jpg "Faturamento")
![Faturamento Detalhe](/uploads/faturamento-detalhe.jpg "Faturamento Detalhe")
![Faturamento Gerado](/uploads/faturamento-gerado.jpg "Faturamento Gerado")

	Fatura
![Fatura](/uploads/fatura.jpg "Fatura")

# Processamento

## Gerar Boleto

	Emissão de Boleto
	
![Impressao Boleto](/uploads/impressao-boleto.jpg "Impressao Boleto")
![Boleto Impresso](/uploads/boleto-impresso.jpg "Boleto Impresso")
![Dados Bancarios](/uploads/dados-bancarios.jpg "Dados Bancarios")

	Gerando Arquivo de Remessa
	
![Gerando Remessa](/uploads/gerando-remessa.jpg "Gerando Remessa")
![Arquivo](/uploads/arquivo.jpg "Arquivo")

	Processando Retorno do banco

## Manual
		Digitação Manual de titulos


	Gerar Arquivo Remessa
	
# Retorno
