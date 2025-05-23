1. Configuração do Ambiente Azure
Criar um Resource Group na Azure para agrupar todos os recursos

Provisionar um Azure Data Factory (ADF)

Criar uma conta de Azure Data Lake Storage Gen2 (ADLS Gen2)

2. Configuração do Integration Runtime
No Azure Data Factory:

Navegar até "Manage" > "Integration Runtimes"

Criar um novo "Self-hosted Integration Runtime"

Baixar e instalar o software em uma máquina local com acesso ao SQL Server on-premises

Registrar o Integration Runtime com a chave de autenticação

3. Criação de Linked Services
Linked Service para SQL Server on-premises:

Tipo: SQL Server

Usar o Integration Runtime criado

Configurar conexão com autenticação SQL

Testar a conexão

Linked Service para Azure Data Lake Storage Gen2:

Tipo: Azure Data Lake Storage Gen2

Método de autenticação: Account Key

Especificar a conta de armazenamento

4. Criação de Datasets
Dataset de origem (SQL Server):

Definir o esquema da tabela de origem

Configurar query ou nome da tabela

Dataset de destino (ADLS Gen2):

Formato: DelimitedText (TXT)

Configurar caminho para a camada raw/bronze

Definir delimitador (vírgula, ponto-e-vírgula, etc.)

5. Criação da Pipeline
Adicionar atividade Copy Data:

Configurar origem como o dataset SQL Server

Configurar destino como o dataset ADLS Gen2

Definir mapeamento de colunas

Configurar parâmetros para tornar a pipeline reutilizável:

Nome da tabela de origem

Nome do arquivo de destino

Caminho de destino

6. Validação e Publicação
Validar a pipeline usando o botão "Validate"

Corrigir eventuais erros

Publicar todas as alterações

7. Execução e Monitoramento
Disparar a pipeline manualmente para teste

Monitorar a execução na aba "Monitor"

Verificar os arquivos criados no Data Lake Storage
