# ProductClient

Este aplicativo é um exemplo de uma aplicação Angular. Trata-se de um app que consome uma API simples que disponibiliza um CRUD de produtos.

## Criar e executar a API

- No diretório de preferência, crie uma pasta para guardar os arquivos necessários para a API;
- Dentro da pasta criada, execute o comando "npm init -y". Esse comando irá criar um arquivo chamado "package.json" que conterá algumas configurações, incluindo os comandos para inicialização da API e a versão usada do JSON Server.
- Ainda dentro da mesma pasta, execute o comando "npm i json-server". Esse comando irá adicionar todas as dependências para que a API seja executada, além de adicioná-las ao arquivo "package.json".
- Para criar a API, é necessário um arquivo .json que será usado como base. Abaixo, segue o arquivo utilizado neste projeto;
![image](https://user-images.githubusercontent.com/62080317/232638407-a7869752-8651-4be0-8820-22031873f2dd.png)
  - Basicamente, quando definimos a propiedade "products", estamos definindo um end-point para nossa API. Então por exemplo, ao fazer uma requisição para localhost:3001/products do tipo GET, o que teremos é a listagem dos produtos definidos no arquivo. Também é possível executar qualquer outra requisição para este mesmo endpoint, como, por exemplo, um POST para salvar um novo produto ou um PUT para atualizar um produto existente.
- No arquivo "package.json", Em "scripts", adicione o comando "json-server --watch db.json --port 3001". Esté comando serve para informar que, quando inicializado, o servidor irá monitorar o arquivo db.json e disponibilizará a API na porta 3001;
- Para executar a API, use o comando "npm start".
## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
