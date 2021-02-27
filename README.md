# Books API

O objetivo deste projeto é aprender como consumir uma API e manipular os dados de acordo com a necessidade.

A API foi criada através do serviço de mockapi.io e pode ser acessada pelo link: https://603ac088f1d6aa0017a10faf.mockapi.io/api/books

Este projeto possui 5 desafios básicos:

1. retornar um **Array** com os autores dos livros
2. retornar somente os livros cujo idioma seja **português**
3. retornar somente os livros com o **valor** **menor** que **40.0**
4. retornar os livros com o número de **páginas maior** que **400** e cujo **idioma** seja **inglês**
5. retornar os livros do autor **Robert Martin C.**

```
.
├── challenges
│   ├── 1
│   │   └── challenge1.js
│   ├── 2
│   │   └── challenge2.js
│   ├── 3
│   │   └── challenge3.js
│   ├── 4
│   │   └── challenge4.js
│   └── 5
│       └── challenge5.js
```

Deve ser utilizado a bilioteca [axios](https://www.npmjs.com/package/axios) para realizar as requisições para a API.

## Como iniciar os desafios

Instalar as dependencias

```
$ npm install
```

Para executar os desafios, basta executar o comando, dentro do diretório correspondente. Ex.:

```
// challenges/1/
$ node challenge1.js
```

Como realizar uma requisição para a API através do axios?

```
const axios = require("axios");
const config = require("../../config");

axios.get(config.booksApiUrl)
  .then(response => {
    // ...resolva o desafio
  });
```

Para facilitar a visualização no terminal, utilize o logger para isso.
Ex.:

```
const logger = require("../../helpers/logger");

logger.log(output);
```

Boa sorte :)
