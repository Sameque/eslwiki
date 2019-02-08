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
A integração bancária tem a finalidade de integrar a parte finaceiro do sistema com o banco atraves de arquivos de remessa e retorno.

Operacionalmente o usuário gera um arquivo de remessa atraves do sistema, processa esse arquivo no site/aplicação do banco que devolve um arquivo de retorno para o usuário contendo o resultado. 
O usuário processa o arquivo no sistema que dependendo da ocorrencia lançada pelo banco executa a baixa ou não do(s) titulo(s).

![Remessa Retorno](/uploads/remessa-retorno.png "Remessa Retorno")

Os títulos podem ter origem pelo processo automático de faturamento de movimentos ou lançados manualmente pelo usuário.

# Origem
## Faturamento Cliente
O cliente fatura os fretes gravados no sistema e gerando um título, imprime o boleto para enviar ao seu cliente e gera o arquivo de remessa para processar no banco.

	Minutas geradas no sistema

![Minuta Gerada](/uploads/minuta-gerada.jpg "Minuta Gerada") ![Minuta Gerada 01](/uploads/minuta-gerada-01.jpg "Minuta Gerada 01")
(Modulo Transporte >> Menu Operacional >> Emissão de Frete >> Botão Incluir)

![Minutas](/uploads/minutas.jpg "Minutas")
(Modulo Transporte >> Menu Operacional >> Emissão de Frete)


	Faturamento

![Faturamento](/uploads/faturamento.jpg "Faturamento")
(Modulo Transporte >> Financeiro >> Fechamento Contas a Receber >> Faturamento Cliente)

![Faturamento Detalhe](/uploads/faturamento-detalhe.jpg "Faturamento Detalhe")
![Faturamento Gerado](/uploads/faturamento-gerado.jpg "Faturamento Gerado")
(Modulo Transporte >> Financeiro >> Fechamento Contas a Receber >> Faturamento Cliente >> Botão Detalhe)

	Fatura
A pos faturar os movimentos a fatura fica disponivel para consulta no modulo financeiro, conforme imagem a baixo.
Note qua a fatura não possui dados bancários (nosso número, Contabancária, etc. ), esses dados serão preenchidos automáticamante pelo sistema na impressão do boleto(*1).

![Fatura](/uploads/fatura.jpg "Fatura")
(Modulo Financeiro >> Menu Lançamentos >> Contas a pagar / receber)

# Processamento

## Gerar Boleto

	Emissão de Boleto
O próximo passo é fazer a impressão do boleto que será enviado para o cliente efetuar o pagamento.

![Impressao Boleto](/uploads/impressao-boleto.jpg "Impressao Boleto")
![Boleto Impresso](/uploads/boleto-impresso.jpg "Boleto Impresso")
(Modulo Financeiro >> Menu Lançamentos >> Emissão de Boleto/Fatura)

Observe que apos a impressão os dados bancários são preenchidos.

![Dados Bancarios](/uploads/dados-bancarios.jpg "Dados Bancarios")
(Modulo Financeiro >> Menu Lançamentos >> Contas a pagar / receber)

	Gerando Arquivo de Remessa
	
![Gerando Remessa](/uploads/gerando-remessa.jpg "Gerando Remessa")
![Arquivo](/uploads/arquivo.jpg "Arquivo")

	Processando Retorno do banco

## Manual
		Digitação Manual de titulos


	Gerar Arquivo Remessa
	
# Retorno

# Notas
1. Caso a emprsa não  utilize a impressão de boletos pelo sistema ESL os dados bancários serão gerados no momento da geração do arquivo de remessa (2.2)