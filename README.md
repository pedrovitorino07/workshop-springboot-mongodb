# Workshop Spring Boot com MongoDB 🧪

Este projeto é uma API RESTful desenvolvida com **Spring Boot** e **MongoDB**, como parte de um workshop prático com foco em conceitos essenciais de criação de aplicações web modernas utilizando banco de dados NoSQL.

## 📚 Descrição

A aplicação simula um sistema simples de gerenciamento de usuários e publicações, com as funcionalidades básicas de um CRUD (Create, Read, Update, Delete). O objetivo é demonstrar como integrar o Spring Boot ao MongoDB, utilizando boas práticas de arquitetura e organização de código.

## 🚀 Tecnologias Utilizadas

- **Java 17+**
- **Spring Boot**
  - Spring Web
  - Spring Data MongoDB
- **MongoDB**
- **Maven**
- **Postman (para testes da API)**

## 🗂️ Estrutura do Projeto

src/
└── main/
├── java/
│ └── com.example.workshopmongo/
│ ├── controller/
│ ├── domain/
│ ├── dto/
│ ├── repository/
│ ├── services/
│ └── config/
└── resources/
├── application.properties


## 📌 Funcionalidades

- [x] Cadastro de usuários
- [x] Listagem de todos os usuários
- [x] Atualização de dados de um usuário
- [x] Remoção de usuários
- [x] Cadastro de posts vinculados a um usuário
- [x] Busca de postagens por usuário
- [x] Comentários em posts

## 🔄 Endpoints Principais

### Usuários
- `GET /users` – Listar todos os usuários  
- `GET /users/{id}` – Buscar usuário por ID  
- `POST /users` – Inserir novo usuário  
- `PUT /users/{id}` – Atualizar dados de um usuário  
- `DELETE /users/{id}` – Deletar usuário

### Postagens
- `GET /posts` – Listar todas as postagens  
- `GET /posts/{id}` – Buscar postagem por ID  
- `GET /posts/titlesearch?text={texto}` – Buscar postagens por título  
- `GET /posts/fullsearch?text={texto}&minDate={data1}&maxDate={data2}` – Buscar postagens por texto e intervalo de datas

## ⚙️ Configuração

1. Clone o projeto:
```bash
git clone https://github.com/pedrovitorino07/workshop-springboot-mongodb.git
cd workshop-springboot-mongodb

2. Configure o MongoDB local ou use o Atlas, e edite o application.properties:
spring.data.mongodb.database=workshopmongo
spring.data.mongodb.uri=mongodb://localhost:27017

3. Execute o projeto
```bash
./mvnw spring-boot:run

4. A API estará disponível em:
http://localhost:8080



