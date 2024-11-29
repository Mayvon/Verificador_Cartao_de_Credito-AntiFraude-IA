Aqui está a descrição em Markdown para o seu repositório no GitHub. Ela resume o funcionamento do aplicativo e como configurar o ambiente:

```markdown
# Desafio 1 - Azure - Fake Docs

Este projeto foi desenvolvido como parte do desafio de integração de tecnologias na plataforma Digital Innovation One (DIO). O objetivo é construir uma aplicação capaz de realizar upload de arquivos de imagem (PNG, JPG, JPEG) para o Azure Blob Storage, processar os documentos utilizando a API do Azure Document Intelligence para análise de cartões de crédito e exibir as informações extraídas na interface.

## Funcionalidades

- **Upload de Arquivos**: O usuário pode fazer o upload de arquivos de imagem diretamente pela interface.
- **Armazenamento em Azure Blob Storage**: Os arquivos enviados são armazenados em um contêiner no Azure Blob Storage.
- **Análise de Cartão de Crédito**: Após o upload, o arquivo é processado com a API `prebuilt-creditCard` do Azure Document Intelligence, que extrai informações como nome do titular, número do cartão, data de validade e banco emissor.
- **Validação Visual**: O resultado da validação é exibido na interface, mostrando as informações extraídas ou indicando que o cartão não é válido.

## Tecnologias

- **Streamlit**: Utilizado para criar a interface web de forma simples e interativa.
- **Azure Blob Storage**: Armazenamento em nuvem para guardar os arquivos de imagem.
- **Azure Document Intelligence**: API do Azure para análise de documentos e extração de dados de cartões de crédito.
- **Python**: Linguagem de programação utilizada no backend.

## Como Usar

### Pré-requisitos

1. Instalar as dependências do projeto:
   ```bash
   pip install -r requirements.txt
   ```

2. Configurar as variáveis de ambiente:
   - Crie um arquivo `.env` na raiz do projeto.
   - Adicione suas credenciais do Azure:
     ```
     ENDPOINT=<your_endpoint>
     SUBSCRIPTION_KEY=<your_subscription_key>
     AZURE_STORAGE_CONNECTION_STRING=<your_storage_connection_string>
     CONTAINER_NAME=<your_container_name>
     ```

### Executando o Projeto

1. Inicie o aplicativo Streamlit:
   ```bash
   streamlit run app.py
   ```

2. Acesse o aplicativo no navegador e faça o upload de um arquivo de imagem (PNG, JPG ou JPEG).
3. O arquivo será enviado para o Azure Blob Storage e processado pela API do Azure Document Intelligence.

### Estrutura de Arquivos

- `app.py`: Arquivo principal que contém a interface do usuário e a lógica de upload e análise.
- `services/blob_service.py`: Função responsável por fazer o upload de arquivos para o Azure Blob Storage.
- `services/credit_card_service.py`: Função que interage com a API do Azure Document Intelligence para analisar os cartões de crédito.
- `utils/Config.py`: Arquivo que carrega as variáveis de configuração, incluindo credenciais do Azure.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
```

Essa descrição cobre as funcionalidades principais, como configurar o ambiente, executar o projeto e uma visão geral da estrutura de arquivos. Se precisar de mais detalhes ou ajustes, é só avisar!
