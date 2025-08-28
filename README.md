# 📌 Spring-Boot-API-Model  

Este projeto é um **template base** para criação de APIs utilizando **Spring Boot** com arquitetura em camadas.  
O objetivo é fornecer um modelo inicial para projetos Java, facilitando a organização do código e a padronização da estrutura.  

---

## 🚀 Tecnologias Utilizadas  

- **Java 17**  
- **Spring Boot 3.5.5**  
  - Spring Web  
  - Spring Data JPA  
- **PostgreSQL**  
- **Lombok**  
- **Maven**  

---

## 📂 Estrutura do Projeto  

O projeto segue a arquitetura em camadas:  
```
src/main/java/br/com/spring/boot/model
│
├── api → Camada de entrada (Controllers / APIs REST)
│
├── dto → Objetos de transferência de dados
│ ├── enums → Enumerações utilizadas nos DTOs
│ ├── request → Objetos usados nas requisições (entrada de dados)
│ └── response → Objetos usados nas respostas (saída de dados)
│
├── exceptions → Classes de exceção e handlers globais
│
├── models → Entidades JPA (mapeamento do banco de dados)
│
├── repositories → Interfaces de acesso a dados (Spring Data JPA)
│
├── services → Regras de negócio e orquestração entre camadas
│
└── utils → Classes utilitárias e helpers
```

---

## ⚙️ Configuração do Projeto  

### Pré-requisitos  
- Java 17+  
- Maven 3.9+  
- PostgreSQL instalado e configurado  

### Configuração do Banco de Dados  
Edite o arquivo **`application.properties`** (ou `application.yml`) e configure sua conexão:  

```
spring.datasource.url=jdbc:postgresql://localhost:5432/seu_banco
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

## ▶️ Executando o Projeto  

1. Clone este repositório:  
   ```bash
   git clone https://github.com/seu-usuario/Spring-Boot-API-Model.git
2. Acesse a pasta do projeto:
   ```
   cd Spring-Boot-API-Model
3. Compile e rode a aplicação:
   ```
   mvn spring-boot:run
4. Acesse a API em:
   ```
   http://localhost:8080

