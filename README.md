## NLW5
Node.js

# Aula 2
### Formas de trabalhar com Banco de dados
* porsager/postgres

* Knex: query builder - rdms driver

* Frameworks ORM > TypeORM: http://typeorm.io

* Sequelize: http://sequelize.org

### Instalando o Type ORM
```
yarn add typeorm reflect-metadata sqlite3
```
### Criando migrations
```
yarn typeorm migration:create -n CreateSettings
```
### Rodando migrations
```
yarn typeorm migration:run
```
### Revertendo migrations
```
yarn typeorm migration:revert
```

## Configurando db connector
* sqlite

Se usa Ubuntu, primeiramente instalar o sqlite ```sudo apt install sqlite```
* Instalar o Plugin do Sqlite com VS > Ctlr + Shift + P > Open SQLite DB
* Beekeeper studio:https://snapcraft.io/install/beekeeper-studio/ubuntu

### Criando entidade
* Adicionado lib uuid
```
yarn add uuid
```
* Adicionando tipagens uuid
```
yarn add @types/uuid -D
```

# Aula 3
*Criação do Service e tratamento de erro ao criar usuário já existente

### Criação da tabela de usuários
```
yarn typeorm migration:create -n CreateUsers
```
```
yarn typeorm migration:run
```

### Criação da tabela de mensagens
```
yarn typeorm migration:create -n CreateMessages
```
```
yarn typeorm migration:run
```

### Requisições:


# Aula 4
### Instalando o Socket.io
```
yarn add socket.io && yarn add @types/socket.io
```
### Instalando o EJS
```
yarn add ejs
```
### Instalando o Socket Client
```
yarn add socket.io-client
```
### Acessando o chat
Lado do Cliente:
http://localhost:3333/pages/client

Lado do Atendente:
http://localhost:3333/pages/admin

### Criando tabela de conexões
```
yarn typeorm migration:create -n CreateConnections
```
```
yarn typeorm migration:run
```
