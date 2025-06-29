# clientes-api-ud

API para gerenciamento de clientes, desenvolvida em Node.js e Express. Este projeto visa fornecer uma interface RESTful para operações de cadastro, consulta, atualização e remoção de clientes, podendo ser facilmente integrada a outros sistemas.

## Funcionalidades

- Cadastro de novos clientes
- Listagem de clientes
- Atualização de dados de clientes
- Remoção de clientes
- Busca de clientes por diferentes critérios

## Tecnologias Utilizadas

- Node.js
- Express
- MongoDB (ou outro banco de dados, caso aplicável)
- Mongoose (se utilizar MongoDB)
- Dotenv para gerenciamento de variáveis de ambiente

## Como executar o projeto

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/robertorj7/clientes-api-ud.git
   cd clientes-api-ud
   ```

2. **Instale as dependências:**
   ```bash
   npm install
   ```

3. **Configure as variáveis de ambiente:**
   - Crie um arquivo `.env` na raiz do projeto e adicione as configurações necessárias, por exemplo:
     ```
     PORT=3000
     DATABASE_URL=mongodb://localhost:27017/clientes
     ```

4. **Inicie o servidor:**
   ```bash
   npm start
   ```
   O servidor estará disponível em `http://localhost:3000`.

## Endpoints Principais

| Método | Rota           | Descrição                    |
|--------|----------------|------------------------------|
| GET    | /clientes      | Lista todos os clientes      |
| POST   | /clientes      | Cria um novo cliente         |
| GET    | /clientes/:id  | Busca um cliente por ID      |
| PUT    | /clientes/:id  | Atualiza um cliente por ID   |
| DELETE | /clientes/:id  | Remove um cliente por ID     |

## Estrutura do Projeto

```
clientes-api-ud/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   └── app.js
├── .env
├── package.json
└── README.md
```