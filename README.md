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
