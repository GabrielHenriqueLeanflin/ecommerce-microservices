# E-commerce com Microerviços

Este projeto é uma plataforma de e-commerce construída com uma arquitetura de microerviços, utilizando Java com Spring Boot para o backend e React para o frontend. Todo o ambiente é orquestrado com Docker.

## - Funcionalidades

*  Cadastro e Login de Usuários (com JWT)
* Listagem de Produtos com Filtros
* Carrinho de Compras
* Checkout Simulado
* Painel Administrativo para Gerenciamento de Produtos

## - Tecnologias Utilizadas

* **Backend:** Java 17, Spring Boot 3, Spring Security, Spring Data JPA
* **Frontend:** React
* **Banco de Dados:** PostgreSQL
* **Containerização:** Docker, Docker Compose
* **Arquitetura:** Microerviços

## - Rodar o Projeto

Este projeto é 100% containerizado, então você **não precisa instalar Java ou Node.js** na sua máquina, apenas o Docker.
1.  **Suba os contêineres na raiz do projeto:**
    ```bash
    docker-compose up --build
    ```

## - Estrutura do Projeto

O projeto é dividido nos seguintes microerviços:

* **/auth-service:** Responsável pelo cadastro, login e gerenciamento de tokens de autenticação (JWT).
* **/product-service:** Gerencia o catálogo de produtos.
* **/order-service:** Processa e gerencia os pedidos dos clientes.
* **/gateway-api:** Ponto de entrada único (API Gateway) para todas as requisições externas.
* **/frontend:** A aplicação React que consome as APIs do backend.

---