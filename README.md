# Projeto Java Spring

Este projeto foi desenvolvido utilizando o framework Spring Boot, seguindo boas práticas e padrões modernos para construção de APIs REST. O objetivo é demonstrar conceitos fundamentais do desenvolvimento web com Java Spring, incluindo arquitetura, persistência de dados e deploy.

## 📌 Tecnologias Utilizadas

- **Java 17**
- **Spring Boot**
- **Spring Data JPA**
- **H2database**
- **Docker & Docker Compose**
- **CI/CD (GitHub Actions)**

## 📚 Conceitos Aprendidos

### 🚀 Desenvolvimento Web e API REST
- Arquitetura Cliente/Servidor
- Protocolo HTTP e JSON
- Padrão REST para API Web

### 🏗️ Estrutura e Padrões de Projeto
- Organização de projeto com Spring REST
- Padrão em camadas: **Controller, Service e Repository**
- Uso de **DTOs (Data Transfer Objects)**

### 🗄️ Persistência de Dados
- Mapeamento objeto-relacional (**ORM**) com JPA/Hibernate
- Relacionamento **N-N** utilizando classe de associação e `@EmbeddedId`
- Consultas SQL personalizadas com **Spring Data JPA (Projections)**
- **Database seeding** para popular dados iniciais
![image](https://github.com/user-attachments/assets/acacb4f4-58d0-4c2b-b57d-bd5378f6344e)

### ⚙️ Configuração e Deploy
- Perfis de projeto (**dev, prod**) e configuração de ambiente
- Uso do **Docker Compose** para ambiente local
- Implementação de **CI/CD** para deploy automatizado
- Configuração de **CORS** para segurança e acesso adequado à API

### 🔗 Design e Implementação de Endpoints
- Uso adequado dos **verbos HTTP** (GET, POST, PUT, DELETE)
- Garantia de **idempotência** nas requisições

### ✨ Endpoints

#### GET games
- localhost:8080/games

#### GET game by ID
- localhost:8080/games/1

#### GET game list
- localhost:8080/lists

#### GET games by list
- localhost:8080/lists/2/games

#### POST list replacement por uma requisição JSON
```
{
    "sourceIndex": 1,
    "destinationIndex": 2
}
```

## ▶️ Como Executar o Projeto

1. Clone este repositório:
   ```sh
   git clone https://github.com/perseu444/dslist.git
   cd dslist
   ```
2. Configure as variáveis de ambiente no arquivo `.env`
3. Execute o projeto localmente com Docker Compose:
   ```sh
   docker-compose up -d
   ```
4. Acesse a API via `http://localhost:8080`



