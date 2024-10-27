# Projeto de API em Flask: Sorteio de 6 Dezenas

Este projeto é a minha primeira API desenvolvida em Python, como parte do meu processo de aprendizado sobre Python e suas bibliotecas. A API foi criada usando o framework Flask e retorna 6 dezenas sorteadas, com a configuração de CORS para permitir requisições do front-end tanto no ambiente de desenvolvimento quanto no de deploy.

## Tecnologias Utilizadas

- Python: Linguagem de programação principal.
- Flask: Framework leve para construção de APIs.
- Flask-CORS: Para configurar o CORS (Cross-Origin Resource Sharing).

## Funcionalidades

- A API retorna 6 dezenas sorteadas ao fazer uma requisição `GET` para o endpoint `/api/sort-number`.
- Configuração de CORS:
  - Permite requisições do ambiente de desenvolvimento (http://localhost:3000).
  - Configurada também para aceitar o link de produção/deploy.

## Endpoints

Este endpoint gera e retorna uma lista de 6 dezenas aleatórias entre 1 a 60 .

```
method: GET

endpoint: /api/sort-number
```

### Exemplo de resposta:

```json
  {
    [5, 12, 23, 34, 45, 56]
  }
```

## Deploy

O deploy da API foi feito na plataforma [Railway](https://railway.app/), onde aprendi bastante sobre como configurar e hospedar uma aplicação em Flask.

Após o deploy, foi necessário ajustar a configuração de CORS para permitir requisições da URL de produção conforme apresentado acima.

Este processo de deploy me proporcionou muito aprendizado sobre o ciclo de vida de uma aplicação, desde a criação local até a disponibilização em um ambiente de produção.

Se você quiser testar a API em produção, ela está disponível [aqui](https://api-number.up.railway.app/api/sort-number). Caso queira testar a API integrada ao front-end, [clique aqui](https://sena-iota.vercel.app).
