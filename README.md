<<<<<<< HEAD
# Jitterbit Technical Test

Este repositório contém:

- Implementação da API de pedidos em Node.js
- Respostas do teste teórico em JavaScript

# Order API

API desenvolvida em Node.js para gerenciamento de pedidos.

Este projeto foi criado como parte de um teste técnico e permite realizar operações de CRUD de pedidos.

## Tecnologias utilizadas

- Node.js
- Express
- MongoDB
- Mongoose

## Instalação

1. Clone o repositório

```
git clone https://github.com/seu-usuario/order-api.git
```

2. Entre na pasta do projeto

```
cd order-api
```

3. Instale as dependências

```
npm install
```

4. Execute o projeto

```
node server.js
```

A API irá rodar em:

```
http://localhost:3000
```

---

# Endpoints

## Criar pedido

POST

```
/order
```

Exemplo de request:

```json
{
  "numeroPedido": "v10089015vdb-01",
  "valorTotal": 10000,
  "dataCriacao": "2023-07-19T12:24:11.5299601+00:00",
  "items": [
    {
      "idItem": "2434",
      "quantidadeItem": 1,
      "valorItem": 1000
    }
  ]
}
```

Resposta:

```json
{
  "orderId": "v10089015vdb",
  "value": 10000,
  "creationDate": "2023-07-19T12:24:11.529Z",
  "items": [
    {
      "productId": 2434,
      "quantity": 1,
      "price": 1000
    }
  ]
}
```

---

## Buscar pedido

GET

```
/order/:orderId
```

Exemplo:

```
GET /order/v10089015vdb
```

---

## Listar pedidos

GET

```
/order/list
```

---

## Atualizar pedido

PUT

```
/order/:orderId
```

---

## Deletar pedido

DELETE

```
/order/:orderId
```

---

# Estrutura do projeto

```
order-api
│
├── models
│   └── Order.js
│
├── routes
│   └── orderRoutes.js
│
├── server.js
├── package.json
└── README.md
```

---

# Banco de dados

Foi utilizado **MongoDB Atlas** como banco de dados.

Os dados são armazenados na coleção `orders`.

Estrutura do documento:

```json
{
  "orderId": "string",
  "value": number,
  "creationDate": "date",
  "items": [
    {
      "productId": number,
      "quantity": number,
      "price": number
    }
  ]
}
```
=======
# order-api
>>>>>>> c2b9d7a9365a0f01729309e9176aeeb9badab6de

## Estrutura do projeto

- order-api → implementação da API
- teste-teorico → respostas do teste teórico
