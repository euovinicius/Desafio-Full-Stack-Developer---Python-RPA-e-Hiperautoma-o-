# Portal da Transparência Automation

## Sobre o Código

Este projeto é uma automação web feita com Playwright que realiza as seguintes funções:

- Acessa o Portal da Transparência e navega até a consulta de "Pessoas Físicas e Jurídicas".
- Insere parâmetros (Nome, Filtro de Busca, CPF ou NIS) e realiza a busca.
- Coleta os dados disponíveis na tela "Pessoa Física - Panorama da relação da pessoa com o Governo Federal".
- Captura uma imagem da tela como evidência e converte para Base64.
- Para cada benefício encontrado (Auxílio Brasil, Auxílio Emergencial, Bolsa Família), acessa os detalhes e coleta as informações.
- Encerra a automação e gera um arquivo JSON contendo os dados coletados e a imagem Base64.
-  Funciona em modo headless e permitir execuções simultâneas .

## Tecnologias utilizadas

- Python 3.10+
- Playwright (com suporte opcional ao Stealth Mode)
- Concurrent Futures (ProcessPoolExecutor)
- Pillow (para manipulação de imagens)


![image](https://github.com/user-attachments/assets/f5c3e64b-695c-448d-aee4-9da8f08dc59b)

