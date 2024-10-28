Teste de RPA para Download e Processamento de Dados CNPJ
Objetivo: Automatizar o download e processamento mensal dos dados do CNPJ usando UiPath.
Contexto Atual
Mensalmente, um membro do nosso time operacional precisa acessar o portal https://dados.gov.br/dados/conjuntos-dados/cadastro-nacional-da-pessoa-juridica---cnpj. Se a data de última alteração dos dados for posterior à data do último download realizado no mês anterior, ele deve proceder com o download manual dos seguintes arquivos:
•
Dicionário de Dados do Cadastro Nacional da Pessoa Jurídica (Pdf)
•
Cnaes (Zip)
•
Empresas0 a Empresas9 (Zip)
•
Estabelecimentos0 a Estabelecimentos9 (Zip)
•
Motivos (Zip)
•
Municípios (Zip)
•
Países (Zip)
•
Qualificações (Zip)
•
Simples (Zip)
•
Sócios0 a Sócios9 (Zip)
Após o download, ele deve descompactar os arquivos, manter os nomes e extensões originais, remover os arquivos ZIP para economizar espaço e enviar um e-mail ao departamento de TI informando que o trabalho foi concluído. Por mais que seja um processo mensal, é um processo que é demorado e repetitivo, por isso precisamos de uma solução de RPA para automatizá-lo.
Tarefas para Automação
1.
Verificar Data de Atualização:
o
Acessar o portal e verificar se a data de última alteração é posterior à data do último download.
2.
Realizar Download:
o
Se a data for mais recente, fazer o download dos arquivos listados acima.
3.
Processar Arquivos:
o
Descompactar os arquivos baixados, mantendo os nomes e extensões originais.
o
Remover os arquivos ZIP baixados.
4.
Notificar TI:
o
Enviar um e-mail ao departamento de TI informando que os arquivos estão disponíveis no diretório de rede.
Nota: Automatize o processo manual descrito acima utilizando UiPath para reduzir o tempo de execução, que atualmente é de cerca de 2 horas. Observe que o portal do governo pode apresentar instabilidade ocasional.
