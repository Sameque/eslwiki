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

Os fretes são gerados no modulo de Transportes.

![Minuta Gerada](/uploads/minuta-gerada.jpg "Minuta Gerada") ![Minuta Gerada 01](/uploads/minuta-gerada-01.jpg "Minuta Gerada 01")
(Modulo Transporte >> Menu Operacional >> Emissão de Frete >> Botão Incluir)

![Minutas](/uploads/minutas.jpg "Minutas")
(Modulo Transporte >> Menu Operacional >> Emissão de Frete)


	Faturamento

Apos emissão os fretes ficam disponíveis para faturamento.

![Faturamento](/uploads/faturamento.jpg "Faturamento")
(Modulo Transporte >> Financeiro >> Fechamento Contas a Receber >> Faturamento Cliente)

![Faturamento Detalhe](/uploads/faturamento-detalhe.jpg "Faturamento Detalhe")
![Faturamento Gerado](/uploads/faturamento-gerado.jpg "Faturamento Gerado")
(Modulo Transporte >> Financeiro >> Fechamento Contas a Receber >> Faturamento Cliente >> Botão Detalhe)

	Fatura
A pos faturar os movimentos a fatura fica disponivel para consulta no modulo financeiro, conforme imagem a baixo.
Note qua a fatura não possui dados bancários (nosso número, Contabancária, etc. ), esses dados serão preenchidos automáticamante pelo sistema na impressão do boleto(*1).

(TRUCAR IMAGEM)
![Fatura](/uploads/fatura.jpg "Fatura")
(Modulo Financeiro >> Menu Lançamentos >> Contas a pagar / receber)

		Digitação Manual de titulos

Alem do faturamento de fretes é possível lançar faturas manualmente, basta o ususário acessar a tela do contas a pagar/receber, clicar no botão novo, digitar as informaçõe do título e gravar.

![Faturamento Manual](/uploads/faturamento-manual.jpg "Faturamento Manual")
(Modulo Transporte >> Financeiro >> Fechamento Contas a Receber >> Faturamento Cliente)
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

Agora precisamos gerara o arquivo de remessa e enviar para o banco.

![Gerando Remessa](/uploads/gerando-remessa.jpg "Gerando Remessa")
(Modulo Financeiro >> Menu Cobrança >> Enviar títulos a receber)

![Arquivo](/uploads/arquivo.jpg "Arquivo")
(imagem do arquivo gerado pelo sistema)

	Processando Retorno do banco

Apos processar no site/aplicação do banco é preciso baixar o arquivo de retorno e atualizar os títulos conforme retorno do banco.
Esse processo é muito importante pois no arquivo de retorno possui as ocorrencias lançadas pelo banco para cada título.


# Notas
1. Caso a emprsa não  utilize a impressão de boletos pelo sistema ESL os dados bancários serão gerados no momento da geração do arquivo de remessa (2.2)