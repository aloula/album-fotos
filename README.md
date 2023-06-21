# Álbum de Fotos

Aplicação Node.js com integração para a [Google Photos Library API](https://developers.google.com/photos).

Essa aplicação se conecta ao Google Photos através de OAuth 2.0 e mostra as fotos do usuário como um álbum de fotos online.

A aplicação é construida com [Express.js](https://expressjs.com/) e [Material Design Lite](https://getmdl.io/).


## Visão Geral

Esta é uma aplicação web que permite ao usário carregar suas fotos do Google Fotos, pesquisar por categorias e datas e visualizar as imagens em slideshow.


## Configuração

Antes de rodas a aplicação, você deve configurar as credentias OAuth 2.0 no Google Developers [get started guide](https://developers.google.com/photos/library/guides/get-started)

1. Configure um projeto Google Developers e habilite **Google Photos Library API**.
2. No seu projeto, configure uma credencial OAuth credentials para Web Server. Configure uma origem Javascript para `http://localhost:8080` e uma URL autorizada para redirect como `http://locahost:8080/auth/google/callback` se estiver rodando a aplicação localmente.
3. O console mostrará suas credencias, adicione o `Client ID` e `Client secret` no arquivo `config_copy.js` e renomei-o para `config.js`:

```
// The OAuth client ID from the Google Developers console.
config.oAuthClientID = 'ADD YOUR CLIENT ID';

// The OAuth client secret from the Google Developers console.
config.oAuthclientSecret = 'ADD YOUR CLIENT SECRET';
```

4. Instale as dependências:
`$ npm install`

5. Execute a aplicação:
`$ node app.js`

6. Abra ser navegador [http://localhost:8080](http://localhost:8080)

