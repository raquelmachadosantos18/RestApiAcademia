# RestApiAcademia
Neste projeto, você irá ver um servidor json (Json-server) onde irá conter 3 rotas com 4+ dados nas quais o usuário poderá realizar o GET, POST, PUT, DELETE. Projeto individual no Módulo 3 - Resilia

Procedimento de instalação
Criar uma pasta e colocar o nome desejado

npm init -y

npm i json-server

Criar o arquivo db.json que será usado como o 'banco de dados'

No package.json na parte scripts "dev": "json-server --watch db.json --port 3000" e apague o anterior que ja existe lá.

Para executar, basta digitar npm run dev

Criar um arquivo: server.js

Inserir o js da documentação no server.js:

// server.js

const jsonServer = require('json-server')

const server = jsonServer.create()

const router = jsonServer.router('db.json' )

const middlewares = jsonServer.defaults()

server.use(middlewares)

server.use(router)

server.listen(3000, () => { console.log('JSON Server is running') })

No Terminal, inserir o comando da documentação para executar o JS acima:

npm install json-server --save-dev //Instalação do servidor local

Executar o comando no terminal para execução do node:

node server.js

- no projeto foi ultizidado o Postman para o teste da Api

*Acesso pelo render
https://restapiacademia.onrender.com 
