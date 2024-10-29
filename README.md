## A documentação está incluída na pasta Documentação

**Teste de RPA para Download e Processamento de Dados CNPJ**

Objetivo: Automatizar o download e processamento mensal dos dados do CNPJ usando UiPath.
Tarefas para Automação
1.Verificar Data de Atualização:
Acessar o portal e verificar se a data de última alteração é posterior à data do último download.
2.Realizar Download:
Se a data for mais recente, fazer o download dos arquivos listados acima.
3.Processar Arquivos:
Descompactar os arquivos baixados, mantendo os nomes e extensões originais.
Remover os arquivos ZIP baixados.
4.Notificar TI:
Enviar um e-mail ao departamento de TI informando que os arquivos estão disponíveis no diretório de rede.

### Modelo

**Robotic Enterprise UIPATH**

- Construído com base no modelo de Processo de Negócio Transacional
- Utiliza o layout de Máquina de Estado para as fases do projeto de automação
- Oferece registro de alto nível, tratamento de exceções e recuperação
- Mantém configurações externas no arquivo Config.xlsx
- Obtém dados de transação do arquivo Transactions.xlsx (processo linear)
- Captura screenshots em caso de exceções do sistema

### Instruções a verificar

1. Verifique o arquivo Config.xlsx e adicione/customize quaisquer campos e valores necessários
2. Verifique o arquivo Transaction.xlsx e adicione uma data para o último download realizado
3. Verifique o arquivo ResourceNames.xlsx e adicione/remova os recursos que deseja que o processo realize o donwload
4. Configure o workflow _4.NotificaTI.xaml_ com o seu e-mail que está habilitado para envio SMTP ou Outlook
5. Verique se a extensão do UiPath está corretamente instalada no navegador Edge
