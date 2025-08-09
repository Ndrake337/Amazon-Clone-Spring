# 🛒 Amazon Clone - Backend

Este projeto é um **clone simplificado da Amazon** criado com foco em **estudos** e **treinamento para vaga de desenvolvedor backend**.  
Ele cobre conceitos essenciais de **Java**, **Spring Boot**, **Kotlin**, **Quarkus**, **Kafka**, **AWS** e práticas modernas de desenvolvimento como **DDD**, **TDD**, **Clean Architecture** e **DevOps**.

---

## ✅ Objetivos
- Criar uma plataforma de e-commerce com arquitetura de microserviços.
- Implementar autenticação (OAuth2/JWT).
- Integrar com mensageria (SQS e Kafka).
- Criar mock de pagamentos em Kotlin/Quarkus.
- Utilizar serviços da AWS (ECS, EKS, RDS, DynamoDB, S3, etc.).
- Aplicar boas práticas de engenharia de software (SOLID, Clean Code, Design Patterns).

---

## 🏗️ Arquitetura

A arquitetura segue o modelo **Clean Architecture + Microservices**:

- **Product Service**: CRUD de produtos.
- **Order Service**: Gestão de pedidos.
- **Payment Service** (Kotlin + Quarkus): Processamento de pagamentos (mock).
- **Auth Service**: Autenticação e autorização.
- **Message Broker**:
  - Kafka (ordens e pagamentos).
  - AWS SQS (notificações).
- **Gateway API**: Entrada única para todos os serviços.
- **Infraestrutura**: AWS ECS/EKS, Terraform para IaC.
- **Observabilidade**: Prometheus, Grafana, Splunk.

---

## 🛠️ Tecnologias
- **Linguagens**: Java 17, Kotlin
- **Frameworks**:
  - Spring Boot, Spring Cloud, Spring Security, Spring Data JPA
  - Quarkus (para serviço de pagamentos)
- **Mensageria**: Kafka, AWS SQS
- **Banco de Dados**: PostgreSQL (prod), H2 (testes), DynamoDB
- **Infra**: AWS ECS/EKS, Terraform, Kubernetes
- **CI/CD**: GitHub Actions
- **Testes**: JUnit5, Mockito, RestAssured
- **Boas práticas**: SOLID, Clean Code, Clean Architecture

---

## 📂 Estrutura do Projeto

**A CONSTRUIR**

---

## ⚙️ Como Rodar Localmente

### Pré-requisitos
- Java 17+
- Maven 3.8+
- Docker e Docker Compose
- Kafka e Zookeeper (para mensageria local)

### Passos
```bash
# 1. Clonar repositório
git clone https://github.com/Ndrake337/Amazon-Clone-Spring.git

# 2. Entrar na pasta do projeto
cd Amazon-Clone-Spring

# 3. Subir dependências (Kafka, DB, etc.)
docker-compose up -d

# 4. Rodar a Aplicação
./mvnw spring-boot:run
```
---

## 🧪 Testes

Rodar testes unitários e de integração:

```bash
./mvnw test
```

---

## 📌 Roadmap

- Criar CRUD de produtos (Java + Spring Boot)

- Criar CRUD de pedidos

- Implementar autenticação com JWT

- Configurar Kafka e publicar eventos

- Criar mock de pagamentos (Kotlin + Quarkus)

- Deploy AWS ECS/EKS via Terraform

- Adicionar observabilidade (Prometheus + Grafana)

- CI/CD no GitHub Actions

## 📄 Licença

Projeto para fins educacionais. Nenhuma afiliação com a Amazon.com, Inc.
