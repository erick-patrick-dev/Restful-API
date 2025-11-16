# Restful-API

Uma API REST desenvolvida em Node.js para gerenciamento de dados de pessoas.

## 📋 Descrição

Este projeto implementa uma API RESTful básica utilizando Node.js, permitindo operações CRUD (Create, Read, Update, Delete) em dados de pessoas.

## 🚀 Tecnologias

- **Node.js** - Runtime JavaScript
- **Express.js** - Framework web (presumido pela estrutura)
- **.env** - Gerenciamento de variáveis de ambiente

## 📁 Estrutura do Projeto

```
Restful-API/
├── .env                 # Variáveis de ambiente
├── .gitignore          # Arquivos ignorados pelo Git
├── index.js            # Arquivo principal da aplicação
├── package.json        # Dependências e scripts do projeto
├── models/
│   └── Person.js       # Modelo de dados para Person
└── routes/
    └── personRoutes.js # Rotas da API para Person
```

## 🔧 Instalação

1. Clone o repositório:
```bash
git clone <seu-repositorio>
cd Restful-API
```

2. Instale as dependências:
```bash
npm install
```

3. Configure as variáveis de ambiente:
Crie ou edite o arquivo `.env` com as variáveis necessárias:
```
PORT=3000
NODE_ENV=development
```

## ▶️ Como Executar

```bash
npm start
```

A API estará disponível em `http://localhost:3000`

## 📡 Endpoints da API

### Pessoas (Person)

- `GET /persons` - Listar todas as pessoas
- `GET /persons/:id` - Obter pessoa por ID
- `POST /persons` - Criar nova pessoa
- `PUT /persons/:id` - Atualizar pessoa
- `DELETE /persons/:id` - Deletar pessoa

## 📝 Exemplo de Requisição

```json
{
  "name": "João Silva",
  "email": "joao@example.com",
  "age": 30
}
```

## 📌 Variáveis de Ambiente

Configurar no arquivo `.env`:
- `PORT` - Porta da aplicação (padrão: 3000)
- `NODE_ENV` - Ambiente (development/production)