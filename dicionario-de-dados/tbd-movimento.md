<!-- TITLE: tbdMovimento-->

	Essa tabela guarda a maioria das informações referente ao movimetno (CT-e/Minuta/NFSe)

				
|Coluna 	|Tipo de Dados 	|Tamanho/Precisão,Escala 	| Descrição|
| ------------- |  ------------- |  ------------- | ------------- | 			
|id_Movimento                            |INT       |--        |Chave primária|
|id_Transportadora                       |INT       |--        |Chave estrangeira referente a Transportadora|
|id_Cliente                              |INT       |--        |Chave estrangeira referente a filial/empresa logada no momento da geração do documento ou empresa selecionada|
|id_TransportadoraServico                |INT       |--        |Chave estrangeira referente a tabela de preço utilizada|
|qt_prazoentrega                         |CHAR      |6         |Quantidade de prazoentrega|
|id_Cidade                               |INT       |--        |Chave estrangeira referente a Cidade|
|nr_NotaFiscal                           |VARCHAR   |800       |Numero de NotaFiscal|
|ds_Cliente                              |CHAR      |80        |Nome do destinatário. - Esse campo guarda o nome do destinatário no momento da gravação do movimento, caso o cadastro do cliente seja alterado essa campo não é atualizado.|
|ds_Endereco                             |VARCHAR   |70        |Descrição do Endereco|
|ds_Bairro                               |VARCHAR   |30        |Descrição do Bairro|
|ds_Telefone                             |VARCHAR   |30        |Descrição do Telefone|
|ds_Ramal                                |CHAR      |20        |Descrição do Ramal|
|ds_Atencao                              |VARCHAR   |30        |??????.|
|ds_Setor                                |VARCHAR   |30        |Descrição do Setor|
|vl_NotaFiscal                           |DECIMAL   |16,4      |Valor de NotaFiscal|
|dt_EmissaoNotaFiscal                    |DATETIME  |--        |Data de EmissaoNotaFiscal|
|cd_CGCCPF                               |CHAR      |14        |Código/número CGCCPF|
|vl_Dimensao1                            |DECIMAL   |16,4      |Valor de Dimensao1|
|kg_Mercadoria                           |DECIMAL   |16,4      |Kilo da Mercadoria|
|vl_Frete                                |DECIMAL   |16,4      |Valor de Frete|
|vl_Dimensao2                            |DECIMAL   |16,4      |Valor de Dimensao2|
|tp_Frete                                |CHAR      |1         |Tipo de Frete|
|vl_Dimensao3                            |DECIMAL   |16,4      |Valor de Dimensao3|
|nr_Coleta                               |CHAR      |20        |Numero de Coleta|
|qt_Volume                               |INT       |--        |Quantidade de Volume|
|vl_ExcedenteColeta                      |DECIMAL   |16,4      |Valor de ExcedenteColeta|
|dt_PrevisaoEntrega                      |DATETIME  |--        |Data de PrevisaoEntrega|
|ds_Receptor                             |VARCHAR   |50        |Nome do receptor, geralmente que recebeu a carga.|
|vl_ExcedenteEntrega                     |DECIMAL   |16,4      |Valor de ExcedenteEntrega|
|vl_Coleta                               |DECIMAL   |16,4      |Valor de Coleta|
|vl_Entrega                              |DECIMAL   |16,4      |Valor de Entrega|
|nr_DocumentoReceptor                    |CHAR      |15        |Numero de DocumentoReceptor|
|vl_Peso                                 |DECIMAL   |16,4      |Valor de Peso|
|dt_Recepcao                             |DATETIME  |--        |Data de Recepcao|
|hr_Recepcao                             |CHAR      |5         |Hora Recepcao|
|nr_Voo                                  |CHAR      |10        |Numero de Voo|
|dt_Voo                                  |DATETIME  |--        |Data de Voo|
|nr_AWB                                  |CHAR      |20        |Numero de AWB|
|id_Agente                               |INT       |--        |Chave estrangeira referente a Agente|
|vl_TaxasDiversas                        |DECIMAL   |16,4      |Valor de TaxasDiversas|
|vl_Redespacho                           |DECIMAL   |16,4      |Valor de Redespacho|
|hr_Partida                              |CHAR      |5         |Hora Partida|
|pc_Desconto                             |DECIMAL   |16,4      |Porcentagem Desconto|
|hr_Chegada                              |CHAR      |5         |Hora Chegada|
|tp_Desconto                             |CHAR      |1         |Tipo de Desconto|
|pc_Acrescimo                            |DECIMAL   |16,4      |Porcentagem Acrescimo|
|tp_Aprovado                             |CHAR      |1         |Tipo de Aprovado|
|tp_Acrescimo                            |CHAR      |1         |Tipo de Acrescimo|
|vl_Suframa                              |DECIMAL   |16,4      |Valor de Suframa|
|vl_Pedagio                              |DECIMAL   |16,4      |Valor de Pedagio|
|vl_ADValorem                            |DECIMAL   |16,4      |Valor de ADValorem|
|vl_TDA                                  |DECIMAL   |16,4      |Valor de TDA|
|hr_PrevisaoEntrega                      |CHAR      |5         |Hora PrevisaoEntrega|
|vl_FreteAereo                           |DECIMAL   |16,4      |Valor de FreteAereo|
|pc_Comissao                             |DECIMAL   |16,4      |Porcentagem Comissao|
|tp_TransferidoEmail                     |CHAR      |1         |Tipo de TransferidoEmail|
|tp_TransferidoDados                     |CHAR      |1         |Tipo de TransferidoDados|
|ds_Aprovador                            |VARCHAR   |50        |Descrição do Aprovador|
|dt_Coleta                               |DATETIME  |--        |Data de Coleta|
|hr_coleta                               |CHAR      |6         |Hora coleta|
|ds_Coletor                              |VARCHAR   |80        |Descrição do Coletor|
|nr_DocumentoColetor                     |VARCHAR   |30        |Numero de DocumentoColetor|
|cd_Placa                                |CHAR      |8         |Código/número Placa|
|cd_Servico                              |CHAR      |10        |Código/número Servico|
|vl_Desconto                             |DECIMAL   |16,4      |Valor de Desconto|
|vl_Acrescimo                            |DECIMAL   |16,4      |Valor de Acrescimo|
|id_CiaAerea                             |INT       |--        |Chave estrangeira referente a CiaAerea|
|tp_CAPAgente                            |CHAR      |1         |Tipo de CAPAgente|
|tp_CAPCiaAerea                          |CHAR      |1         |Tipo de CAPCiaAerea|
|id_Remetente                            |INT       |--        |Chave estrangeira referente a Remetente|
|tp_Movimento                            |CHAR      |1         |Tipo de Movimento|
|qt_Kilometro                            |INT       |--        |Quantidade de Kilometro|
|tp_CarCliente                           |CHAR      |1         |Tipo de CarCliente|
|tp_CarAgente                            |CHAR      |1         |Tipo de CarAgente|
|ds_Remetente                            |VARCHAR   |80        |Descrição do Remetente|
|id_Seguradora                           |INT       |--        |Chave estrangeira referente a Seguradora|
|id_Fiscal                               |INT       |--        |Chave estrangeira referente a Fiscal|
|id_AgenteEmissor                        |INT       |--        |Chave estrangeira referente a AgenteEmissor|
|cd_IE                                   |CHAR      |20        |Código/número IE|
|ds_Embalagem                            |VARCHAR   |30        |Descrição do Embalagem|
|cd_Cep                                  |CHAR      |8         |Código/número Cep|
|cd_Estado                               |CHAR      |2         |Código/número Estado|
|kg_MercadoriaReal                       |DECIMAL   |16,4      |Kilo da MercadoriaReal|
|cm_Entrega                              |VARCHAR   |255       |Comentário Entrega|
|cm_Coleta                               |VARCHAR   |255       |Comentário Coleta|
|hr_Movimento                            |CHAR      |5         |Hora Movimento|
|ds_Usuario                              |VARCHAR   |50        |Descrição do Usuario|
|tp_RetiraMercadoria                     |CHAR      |1         |Tipo de RetiraMercadoria|
|tp_PagaFrete                            |CHAR      |1         |Tipo de PagaFrete|
|dt_Movimento                            |DATETIME  |--        |Data de Movimento|
|id_Destinatario                         |INT       |--        |Chave estrangeira referente a Destinatario|
|id_ClienteFaturamento                   |INT       |--        |Chave estrangeira referente a ClienteFaturamento|
|cm_Movimento                            |CHAR      |2000      |Comentário Movimento|
|cm_Recepcao                             |VARCHAR   |100       |Comentário Recepcao|
|ds_Transportadora                       |VARCHAR   |40        |Descrição do Transportadora|
|ds_Agente                               |VARCHAR   |80        |Descrição do Agente|
|ds_CiaAerea                             |VARCHAR   |80        |Descrição do CiaAerea|
|tp_CalculaFreteAereo                    |CHAR      |1         |Tipo de CalculaFreteAereo|
|id_Servico                              |INT       |--        |Chave estrangeira referente a Servico|
|tp_TaxaMinimaCiaAerea                   |CHAR      |1         |Tipo de TaxaMinimaCiaAerea|
|nr_Minuta                               |CHAR      |20        |Numero de Minuta|
|tp_CAPAgenteEmissor                     |CHAR      |1         |Tipo de CAPAgenteEmissor|
|vl_AgenteEmissor                        |DECIMAL   |16,4      |Valor de AgenteEmissor|
|cd_NFFatura                             |CHAR      |20        |Código/número NFFatura|
|dt_VencimentoTitulo                     |DATETIME  |--        |Data de VencimentoTitulo|
|id_TabelaPrecoCiaAerea                  |INT       |--        |Chave estrangeira referente a TabelaPrecoCiaAerea|
|id_CidadeDestinatario                   |INT       |--        |Chave estrangeira referente a CidadeDestinatario|
|vl_EntregaAgente                        |DECIMAL   |16,4      |Valor de EntregaAgente|
|tp_DescontoCiaAerea                     |CHAR      |1         |Tipo de DescontoCiaAerea|
|dt_Atualizacao                          |DATETIME  |--        |Data de Atualizacao|
|ds_UsuarioAtualizacao                   |VARCHAR   |50        |Descrição do UsuarioAtualizacao|
|ds_NaturezaMercadoria                   |VARCHAR   |30        |Descrição do NaturezaMercadoria|
|tp_TaxaMinimaTransportadora             |CHAR      |1         |Tipo de TaxaMinimaTransportadora|
|tp_ContaCorrente                        |CHAR      |1         |Tipo de ContaCorrente|
|tp_ImpressoRelacaoCarga                 |CHAR      |1         |Tipo de ImpressoRelacaoCarga|
|id_TransportadoraTerrestre              |INT       |--        |Chave estrangeira referente a TransportadoraTerrestre|
|ds_TransportadoraTerrestre              |VARCHAR   |40        |Descrição do TransportadoraTerrestre|
|id_TabelaTransportadora                 |INT       |--        |Chave estrangeira referente a TabelaTransportadora|
|tp_Categoria                            |CHAR      |1         |Tipo de Categoria|
|id_AgenteColeta                         |INT       |--        |Chave estrangeira referente a AgenteColeta|
|vl_AgenteColeta                         |DECIMAL   |16,4      |Valor de AgenteColeta|
|id_Coletor                              |INT       |--        |Chave estrangeira referente a Coletor|
|ds_AgenteColeta                         |VARCHAR   |80        |Descrição do AgenteColeta|
|tp_Documento                            |CHAR      |1         |Tipo de Documento|
|tp_CAPAgenteColeta                      |CHAR      |1         |Tipo de CAPAgenteColeta|
|vl_FreteAereoAWB                        |DECIMAL   |16,4      |Valor de FreteAereoAWB|
|qt_ImpressaoAWB                         |INT       |--        |Quantidade de ImpressaoAWB|
|ds_Solicitante                          |VARCHAR   |30        |Descrição do Solicitante|
|tp_Correio                              |CHAR      |1         |Tipo de Correio|
|dt_Correio                              |DATETIME  |--        |Data de Correio|
|vl_Correio                              |DECIMAL   |16,4      |Valor de Correio|
|vl_FreteAereoDescontado                 |DECIMAL   |16,4      |Valor de FreteAereoDescontado|
|id_Veiculo                              |INT       |--        |Chave estrangeira referente a Veiculo|
|id_Motorista                            |INT       |--        |Chave estrangeira referente a Motorista|
|tp_CidadeCalculo                        |CHAR      |1         |Tipo de CidadeCalculo|
|tp_Faturado                             |CHAR      |1         |Tipo de Faturado|
|id_Consignatario                        |INT       |--        |Chave estrangeira referente a Consignatario|
|tp_AtualizarWeb                         |CHAR      |1         |Tipo de AtualizarWeb|
|id_FormaPagamento                       |INT       |--        |Chave estrangeira referente a FormaPagamento|
|id_TabelaPrecoCorreio                   |INT       |--        |Chave estrangeira referente a TabelaPrecoCorreio|
|dt_Pagamento                            |DATETIME  |--        |Data de Pagamento|
|kg_CiaAerea                             |DECIMAL   |16,4      |Kilo da CiaAerea|
|id_Embalagem                            |INT       |--        |Chave estrangeira referente a Embalagem|
|cm_MovimentoMinuta                      |VARCHAR   |2000      |Comentário MovimentoMinuta|
|dt_Aviso                                |DATETIME  |--        |Data de Aviso|
|hr_Aviso                                |CHAR      |5         |Hora Aviso|
|ds_NomeAviso                            |VARCHAR   |50        |Descrição do NomeAviso|
|cm_Aviso                                |VARCHAR   |50        |Comentário Aviso|
|tp_FechamentoAgente                     |CHAR      |1         |Tipo de FechamentoAgente|
|ds_RazaoSocial                          |VARCHAR   |80        |Descrição do RazaoSocial|
|id_Correio                              |INT       |--        |Chave estrangeira referente a Correio|
|tp_CAPCorreio                           |CHAR      |1         |Tipo de CAPCorreio|
|qt_VolumeImpressaoAWB                   |INT       |--        |Quantidade de VolumeImpressaoAWB|
|vl_EntregaObrigatoria                   |DECIMAL   |16,4      |Valor de EntregaObrigatoria|
|id_FilialOrigem                         |INT       |--        |Chave estrangeira referente a FilialOrigem|
|id_MovimentoFilial                      |INT       |--        |Chave estrangeira referente a MovimentoFilial|
|nr_Conhecimento                         |CHAR      |20        |Numero de Conhecimento|
|pc_Aliquota                             |DECIMAL   |16,4      |Porcentagem Aliquota|
|id_Campanha                             |INT       |--        |Chave estrangeira referente a Campanha|
|ds_Contato                              |VARCHAR   |60        |Descrição do Contato|
|tp_Cobranca                             |CHAR      |1         |Tipo de Cobranca|
|vl_Tarifa                               |DECIMAL   |16,4      |Valor de Tarifa|
|id_ServicoAereo                         |INT       |--        |Chave estrangeira referente a ServicoAereo|
|cd_ServicoAereo                         |CHAR      |5         |Código/número ServicoAereo|
|id_TipoAgenteEntrega                    |INT       |--        |Chave estrangeira referente a TipoAgenteEntrega|
|id_TipoAgenteColeta                     |INT       |--        |Chave estrangeira referente a TipoAgenteColeta|
|qt_KilometroColeta                      |INT       |--        |Quantidade de KilometroColeta|
|vl_ExcedentePeso                        |DECIMAL   |16,4      |Valor de ExcedentePeso|
|vl_Emergencia                           |DECIMAL   |16,4      |Valor de Emergencia|
|vl_PesoParcial                          |DECIMAL   |16,4      |Valor de PesoParcial|
|vl_ISS                                  |DECIMAL   |16,4      |Valor de ISS|
|pc_ISS                                  |DECIMAL   |16,4      |Porcentagem ISS|
|vl_BreakEven                            |DECIMAL   |16,4      |Valor de BreakEven|
|vl_TarifaAerea                          |DECIMAL   |16,4      |Valor de TarifaAerea|
|vl_TaxasPagarAWB                        |DECIMAL   |16,4      |Valor de TaxasPagarAWB|
|vl_TaxasReceberAWB                      |DECIMAL   |16,4      |Valor de TaxasReceberAWB|
|id_CidadeOrigem                         |INT       |--        |Chave estrangeira referente a CidadeOrigem|
|id_Manifesto                            |INT       |--        |Chave estrangeira referente a Manifesto|
|qt_VolumesLidos                         |INT       |--        |Quantidade de VolumesLidos|
|id_ItemPedidoColeta                     |INT       |--        |Chave estrangeira referente a ItemPedidoColeta|
|qt_KilometroMovimento                   |INT       |--        |Quantidade de KilometroMovimento|
|dt_PrazoEntrega                         |DATETIME  |--        |Data de PrazoEntrega|
|hr_PrazoEntrega                         |CHAR      |5         |Hora PrazoEntrega|
|kg_OutraCategoria                       |DECIMAL   |16,4      |Kilo da OutraCategoria|
|pc_ICMS                                 |DECIMAL   |16,4      |Porcentagem ICMS|
|vl_ICMS                                 |DECIMAL   |16,4      |Valor de ICMS|
|vl_SETCAT                               |DECIMAL   |16,4      |Valor de SETCAT|
|vl_ITR                                  |DECIMAL   |16,4      |Valor de ITR|
|vl_Ademe                                |DECIMAL   |16,4      |Valor de Ademe|
|vl_Despacho                             |DECIMAL   |16,4      |Valor de Despacho|
|nr_ConhecimentoTransportadora           |CHAR      |20        |Numero de ConhecimentoTransportadora|
|id_Status                               |INT       |--        |Chave estrangeira referente a Status|
|cd_Emergencia                           |VARCHAR   |50        |Código/número Emergencia|
|id_ManifestoEntrega                     |INT       |--        |Chave estrangeira referente a ManifestoEntrega|
|dt_Despacho                             |DATETIME  |--        |Data de Despacho|
|dt_Retirada                             |DATETIME  |--        |Data de Retirada|
|dt_Redespacho                           |DATETIME  |--        |Data de Redespacho|
|tp_Redespacho                           |CHAR      |1         |Tipo de Redespacho|
|id_TransportadoraRedespacho             |INT       |--        |Chave estrangeira referente a TransportadoraRedespacho|
|id_RelacaoCarga                         |INT       |--        |Chave estrangeira referente a RelacaoCarga|
|id_ManifestoViagem                      |INT       |--        |Chave estrangeira referente a ManifestoViagem|
|dt_Viagem                               |DATETIME  |--        |Data de Viagem|
|id_RemetenteCentroCusto                 |INT       |--        |Chave estrangeira referente a RemetenteCentroCusto|
|id_TipoMovimento                        |INT       |--        |Chave estrangeira referente a TipoMovimento|
|nr_Referencia                           |CHAR      |255       |Numero de Referencia|
|ds_GrauParentesco                       |VARCHAR   |40        |Descrição do GrauParentesco|
|dt_Cadastro                             |DATETIME  |--        |Data de Cadastro|
|ds_UsuarioCadastro                      |VARCHAR   |50        |Descrição do UsuarioCadastro|
|qt_ImpressaoMinuta                      |INT       |--        |Quantidade de ImpressaoMinuta|
|qt_ImpressaoConhecimento                |INT       |--        |Quantidade de ImpressaoConhecimento|
|qt_ImpressaoEtiquetaRemetente           |INT       |--        |Quantidade de ImpressaoEtiquetaRemetente|
|qt_ImpressaoEtiquetaCiaAerea            |INT       |--        |Quantidade de ImpressaoEtiquetaCiaAerea|
|tp_NotaFiscalServico                    |CHAR      |1         |Tipo de NotaFiscalServico|
|nr_Formulario                           |CHAR      |20        |Numero de Formulario|
|hr_ChegadaCliente                       |CHAR      |5         |Hora ChegadaCliente|
|hr_SaidaCliente                         |CHAR      |5         |Hora SaidaCliente|
|tp_TaxaMinimaCliente                    |CHAR      |1         |Tipo de TaxaMinimaCliente|
|nr_ColetaManual                         |CHAR      |10        |Numero de ColetaManual|
|vl_DespesaManifesto                     |DECIMAL   |16,4      |Valor de DespesaManifesto|
|dt_ImpressaoConhecimento                |DATETIME  |--        |Data de ImpressaoConhecimento|
|hr_ImpressaoConhecimento                |CHAR      |5         |Hora ImpressaoConhecimento|
|vl_FreteCliente                         |DECIMAL   |16,4      |Valor de FreteCliente|
|id_Carreta                              |INT       |--        |Chave estrangeira referente a Carreta|
|tp_EnviarEDI                            |CHAR      |1         |Tipo de EnviarEDI|
|tp_EnviarEDIEmbarque                    |CHAR      |1         |Tipo de EnviarEDIEmbarque|
|id_UsuarioEntrega                       |INT       |--        |Chave estrangeira referente a UsuarioEntrega|
|dt_DigitacaoEntrega                     |DATETIME  |--        |Data de DigitacaoEntrega|
|id_UsuarioCadastro                      |INT       |--        |Chave estrangeira referente a UsuarioCadastro|
|ds_EnderecoEntrega                      |VARCHAR   |80        |Descrição do EnderecoEntrega|
|id_CidadeEntrega                        |INT       |--        |Chave estrangeira referente a CidadeEntrega|
|id_CidadeCalculo                        |INT       |--        |Chave estrangeira referente a CidadeCalculo|
|dt_Previsao                             |DATETIME  |--        |Data de Previsao|
|ds_ContatoPrevisao                      |VARCHAR   |30        |Descrição do ContatoPrevisao|
|cd_PeriodoEntrega                       |CHAR      |2         |Código/número PeriodoEntrega|
|dt_Confirmacao                          |DATETIME  |--        |Data de Confirmacao|
|hr_Confirmacao                          |CHAR      |5         |Hora Confirmacao|
|ds_ContatoConfirmacao                   |VARCHAR   |30        |Descrição do ContatoConfirmacao|
|cd_Imposto                              |CHAR      |4         |Código/número Imposto|
|cd_SerieCTRC                            |CHAR      |3         |Código/número SerieCTRC|
|id_PreManifesto                         |INT       |--        |Chave estrangeira referente a PreManifesto|
|tp_Localidade                           |CHAR      |1         |Tipo de Localidade|
|qt_NotaFiscal                           |INT       |--        |Quantidade de NotaFiscal|
|id_ManifestoTransferencia               |INT       |--        |Chave estrangeira referente a ManifestoTransferencia|
|tp_Manifestado                          |CHAR      |1         |Tipo de Manifestado|
|dt_Ocorrencia                           |DATETIME  |--        |Data de Ocorrencia|
|hr_Ocorrencia                           |CHAR      |5         |Hora Ocorrencia|
|id_NaturezaMercadoria                   |INT       |--        |Chave estrangeira referente a NaturezaMercadoria|
|tp_Averbado                             |CHAR      |1         |Tipo de Averbado|
|pc_DescontoPedagio                      |DECIMAL   |16,4      |Porcentagem DescontoPedagio|
|tp_EDI                                  |CHAR      |1         |Tipo de EDI|
|dt_RecepcaoConfirmacao                  |DATETIME  |--        |Data de RecepcaoConfirmacao|
|hr_RecepcaoConfirmacao                  |CHAR      |5         |Hora RecepcaoConfirmacao|
|tp_EnviarEDICont                        |CHAR      |1         |Tipo de EnviarEDICont|
|tp_EnviarEDISite                        |CHAR      |1         |Tipo de EnviarEDISite|
|tp_EnviarEDIRedespacho                  |CHAR      |1         |Tipo de EnviarEDIRedespacho|
|tp_EnviadoSimphony                      |CHAR      |1         |Tipo de EnviadoSimphony|
|tp_EnviadoRodocred                      |CHAR      |1         |Tipo de EnviadoRodocred|
|ds_XMLEnvioRodocred                     |VARCHAR   |2000      |Descrição do XMLEnvioRodocred|
|ds_RetornoRodocred                      |VARCHAR   |500       |Descrição do RetornoRodocred|
|cm_UTIFile                              |CHAR      |20        |Comentário UTIFile|
|cm_UTIInvoice                           |CHAR      |20        |Comentário UTIInvoice|
|nr_UTIFile                              |CHAR      |20        |Numero de UTIFile|
|nr_UTIInvoice                           |CHAR      |20        |Numero de UTIInvoice|
|tp_EnviarDatasul                        |CHAR      |1         |Tipo de EnviarDatasul|
|tp_DocumentoRecebido                    |CHAR      |1         |Tipo de DocumentoRecebido|
|tp_EnviarDataSulTegma                   |CHAR      |1         |Tipo de EnviarDataSulTegma|
|tp_EnviarEDINovo                        |CHAR      |1         |Tipo de EnviarEDINovo|
|TP_ENVIAREDIGBC                         |CHAR      |1         |Tipo de ENVIAREDIGBC|
|tp_EnviarEDIAverbacao                   |CHAR      |1         |Tipo de EnviarEDIAverbacao|
|tp_EnviarEDIAverb                       |CHAR      |1         |Tipo de EnviarEDIAverb|
|TP_ENVIAREDIPRESSURE                    |CHAR      |1         |Tipo de ENVIAREDIPRESSURE|
|tp_AverbadoATM                          |CHAR      |1         |Tipo de AverbadoATM|
|tp_CanceladoATM                         |CHAR      |1         |Tipo de CanceladoATM|
|tp_EDILupBar                            |CHAR      |1         |Tipo de EDILupBar|
|tp_EnviarEDICTeNFsWalmart               |CHAR      |1         |Tipo de EnviarEDICTeNFsWalmart|
|TP_ENVIAREDIPORTO                       |CHAR      |1         |Tipo de ENVIAREDIPORTO|
|id_TabelaPrecoRedespacho                |INT       |--        |Chave estrangeira referente a TabelaPrecoRedespacho|
|id_TabelaPrecoAgenteEntrega             |INT       |--        |Chave estrangeira referente a TabelaPrecoAgenteEntrega|
|id_TabelaPrecoAgenteColeta              |INT       |--        |Chave estrangeira referente a TabelaPrecoAgenteColeta|
|tp_AverbaATM                            |CHAR      |1         |Tipo de AverbaATM|
|cm_Destinatario                         |VARCHAR   |500       |Comentário Destinatario|
|TP_ENVIADOCONTABILIDADE                 |CHAR      |1         |Tipo de ENVIADOCONTABILIDADE|
|tp_EnviarEDIELT                         |CHAR      |1         |Tipo de EnviarEDIELT|
|tp_MinutaAlterada                       |CHAR      |1         |Tipo de MinutaAlterada|
|tp_EnviarEdiSeguro                      |VARCHAR   |1         |Tipo de EnviarEdiSeguro|
|tp_EnviarEDIPF                          |CHAR      |1         |Tipo de EnviarEDIPF|
|TP_AVERBADOTMARINE                      |CHAR      |1         |Tipo de AVERBADOTMARINE|
|tp_AverbadoPortoSeguro                  |CHAR      |1         |Tipo de AverbadoPortoSeguro|
|tp_IntegradoClaro                       |VARCHAR   |1         |Tipo de IntegradoClaro|
|ds_UltimoRetornoClaro                   |VARCHAR   |300       |Descrição do UltimoRetornoClaro|
|tp_IntegradoClaroEnvioXML               |VARCHAR   |1         |Tipo de IntegradoClaroEnvioXML|
|ds_UltimoRetornoClaroEnvioXML           |VARCHAR   |300       |Descrição do UltimoRetornoClaroEnvioXML|
|dt_BaixaTitulo                          |DATETIME  |--        |Data de BaixaTitulo|
|id_Bancario                             |INT       |--        |Chave estrangeira referente a Bancario|
|tp_AverbadoATMAereo                     |CHAR      |1         |Tipo de AverbadoATMAereo|
|id_IntegracaoAgile                      |INT       |--        |Chave estrangeira referente a IntegracaoAgile|
|tp_EnviarAgile                          |VARCHAR   |1         |Tipo de EnviarAgile|
|dt_UltimoEnvioAgile                     |DATETIME  |--        |Data de UltimoEnvioAgile|
|vl_FreteRedespacho                      |DECIMAL   |9,0       |Valor de FreteRedespacho|
|nr_ConhecimentoRedespacho               |CHAR      |15        |Numero de ConhecimentoRedespacho|
|TP_ENVIAREDIIIMAK                       |CHAR      |1         |Tipo de ENVIAREDIIIMAK|
|tp_ComissaoMotCalculado                 |CHAR      |1         |Tipo de ComissaoMotCalculado|
|tp_EnviarInfraero                       |CHAR      |1         |Tipo de EnviarInfraero|
|TP_ENVIARBRENNTAG                       |CHAR      |1         |Tipo de ENVIARBRENNTAG|
|tp_ICMSManual                           |CHAR      |1         |Tipo de ICMSManual|
|pc_ICMSCalculado                        |DECIMAL   |8,4       |Porcentagem ICMSCalculado|
|tp_IntegradoiTrack                      |CHAR      |1         |Tipo de IntegradoiTrack|
|ds_UltimoRetornoiTrack                  |VARCHAR   |200       |Descrição do UltimoRetornoiTrack|