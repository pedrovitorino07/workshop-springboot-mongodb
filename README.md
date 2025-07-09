# 📦 Workshop Spring Boot com MongoDB

Projeto de uma API REST simples usando **Spring Boot** e **MongoDB**, desenvolvido durante um workshop prático.

## 🔧 Funcionalidades

- CRUD de usuários
- CRUD de postagens
- Comentários em postagens
- Busca por título e por intervalo de datas

## 🚀 Tecnologias

- Java
- Spring Boot
- MongoDB
- Maven

## ▶️ Como rodar

1. Clone o repositório:
```bash
git clone https://github.com/pedrovitorino07/workshop-springboot-mongodb.git
cd workshop-springboot-mongodb
```

2. Configure o MongoDB no application.properties:
```bash
spring.data.mongodb.uri=mongodb://localhost:27017
spring.data.mongodb.database=workshopmongo
```

3. Execute o projeto
```bash
./mvnw spring-boot:run
```

A API estará disponível em: http://localhost:8080
