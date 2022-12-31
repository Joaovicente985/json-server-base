# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth já configurada, feita para ser usada no desenvolvimento das API's nos Projetos Front-end.

## Endpoints

Assim como a documentação do JSON-Server-Auth traz (https://www.npmjs.com/package/json-server-auth), existem 3 endpoints que podem ser utilizados para cadastro e 2 endpoints que podem ser usados para login.

### Cadastro

POST /register <br/>
POST /signup <br/>
POST /users

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.

### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"

### Register Book

Post /books

Para registrar um livro você deve inserir os campos "bookName", "category" e "userId" para referenciar o id do usuário logado, é necessário o uso de um Token para efetuar o registro

### Register Movie

Post /movies

Para registrar um filme você deve inserir os campos "movieName", "category", e userId para referenciar o id do usuário logado, é necessário o uso de um Token para efetuar o registro

### Get All Movies

Get /movies

não é necessário o uso de Token para acessar a lista de filmes cadastrados

### Get All Books

Get /books

não é necessário o uso de Token para acessar a lista de livros cadastrados
