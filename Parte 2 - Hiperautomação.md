# Integração com API do Robô de Consulta - Portal da Transparência

## Descrição

Este projeto realiza uma integração automática com o robô de consulta desenvolvido na Parte 1.  
Ele permite enviar uma requisição via API, armazenar os dados no Google Drive e atualizar um registro centralizado no Google Sheets.

## Funcionalidades

- Robô hospedado em **ender.com**

![image](https://github.com/user-attachments/assets/46479dac-db94-4d4f-83fe-30b19877c72a)

- Realiza requisição à API do robô hospedado em **ender.com** utilizando o **Postman** ou outra ferramenta de automação.

![image](https://github.com/user-attachments/assets/7e5507fb-f212-47b1-b3c0-142a4bd4b6f6)

- Armazena automaticamente o arquivo JSON gerado no **Google Drive**, com nome padrão.
- Atualiza um **Google Sheets** centralizado contendo:
  - Identificador único da consulta
  - Nome
  - CPF
  - Data e hora da consulta
  - Link direto para o arquivo JSON correspondente no Drive

## Tecnologias utilizadas

- API do Activepieces (automação de requisições e processos)
- Postman (teste e envio de requisições)
- Google Drive API (armazenamento de arquivos)
- Google Sheets API (atualização de planilha)
- Robô de consulta desenvolvido em Python e Playwright

## Fluxo geral

1. O usuário envia uma requisição de consulta via API.
2. O Activepieces orquestra o processo:
    - Aguarda a resposta da consulta.
    - Salva o arquivo JSON recebido no Google Drive.
    - Gera o link público de acesso ao JSON.
    - Atualiza a planilha no Google Sheets com todas as informações da consulta.
      
![image](https://github.com/user-attachments/assets/6139c47b-e20e-4b67-9f18-1dc9524e33f4)

## Observações

- O Activepieces foi utilizado para automatizar todo o processo, sem necessidade de intervenção manual.
- O nome do arquivo JSON é gerado de forma padronizada para facilitar a organização.
- O link armazenado na planilha é direto para o arquivo no Drive, facilitando futuras consultas.

## Pré-requisitos

- Conta no Activepieces configurada.
- Conta no Google Drive e Google Sheets com as permissões de API ativadas.
- Postman (ou outra ferramenta) configurado para fazer chamadas POST para o endpoint da API.

