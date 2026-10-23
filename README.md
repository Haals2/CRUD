# CRUD de Produtos

## Descrição
Projeto estressante e desafiador, porem gratificante o resultado feito com dedicaçao. O sistema permite cadastrar, consultar, atualizar e excluir produtos.

## Tecnologias utilizadas
- JavaScript
- Node.js
- Express
- SQLite
- better-sqlite3

## Estrutura do projeto

```text
crud-produtos/
├── app.js
├── crud_banco.sql
├── LojaDB.db
├── package.json
└── README.md
```

## Como executar

1. Instale o Node.js.
2. Abra o terminal na pasta do projeto.
3. Instale as dependências:

   ```bash
   npm install
   ```

4. Verifique se o arquivo `LojaDB.db` está na pasta do projeto.
5. Inicie o servidor:

   ```bash
   node app.js
   ```

6. A API estará disponível em `http://localhost:3000`.

## Rotas da API

| Método | Rota | Função |
|---|---|---|
| GET | `/` | Verificar se a API está funcionando |
| POST | `/produtos` | Cadastrar um produto |
| GET | `/produtos` | Listar os produtos |
| PUT | `/produtos/:id` | Atualizar um produto |
| DELETE | `/produtos/:id` | Excluir um produto |

## Exemplo de produto

```json
{
  "nome": "Teclado mecânico",
  "preco": 149.90,
  "quantidade": 20
}
```

Para as requisições POST e PUT, envie os dados no formato JSON.

## Banco de dados

O banco utilizado é o SQLite, armazenado no arquivo `LojaDB.db`. O arquivo `crud_banco.sql` contém o comando para criar a tabela `Produtos`.

## Observação

As requisições foram testadas no Postman durante o desenvolvimento do projeto.