
# Support-Tickets

Api para controle de tickets, desenvolvida em node, sem dependencias, utilizando .json como database.


## Documentação da API

#### Retorna todos os tickets

```http
  GET http://localhost:3333/tickets
```

#### Adiciona um novo ticket

```http
  POST http://localhost:3333/tickets
```

| Body   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `equipament`      | `string` | **Obrigatório**. O nome do equipamento |
| `description`      | `string` | **Obrigatório**. A descrição do ticket |
| `user_name`      | `string` | **Obrigatório**. Usuário que inclui o ticket |

#### Altera um ticket

```http
  PUT http://localhost:3333/tickets/:id
```

| Body   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `equipament`      | `string` | **Opcional**. O nome do equipamento |
| `description`      | `string` | **Opcional**. A descrição do ticket |


#### Fechar ticket e adicionar solução

```http
  PUT http://localhost:3333/tickets/:id/close
```

| Body   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `solution`      | `string` | **Obrigatório**. A solução do problema |

#### Deletar ticket

```http
  DELETE http://localhost:3333/tickets/:id
```

## Créditos
- [Rocketseat](https://github.com/Rocketseat) - Instituição de educação em tecnologia
-  [Fundamentos NodeJs](https://app.rocketseat.com.br/?type=ALL) - Curso




## Contato
📧 Email: [lucasrop22@gmail.com](mailto:lucasrop22@gmail.com)  
🌐 Linkedin: [lucasrpinto-dev](https://www.linkedin.com/in/lucasrpinto-dev/)  



#### Linguagem Utilizada

![Node.js](https://img.shields.io/badge/node.js-v23.2.0-green)