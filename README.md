# API Rest de cadastro de produtos

## Este projeto é uma API de controle de estoque e cadastramento de produtos desenvolvida usando Java e o framework Spring Boot. A API permite operações CRUD (Create, Read, Update, Delete) em produtos no banco de dados MySQL.

# O que o projeto faz?

## Listar Produtos:
Endpoint: GET /api/produtos
Descrição: Retorna uma lista de todos os produtos no estoque.

## Buscar Produto por ID:
Endpoint: GET /api/produtos/{id}
Descrição: Retorna os detalhes de um produto específico com base no ID.

## Adicionar Novo Produto:
Endpoint: POST /api/produtos
Descrição: Adiciona um novo produto ao estoque.

## Atualizar Produto:
Endpoint: PUT /api/produtos/{id}
Descrição: Atualiza as informações de um produto existente.

## Deletar Produto:
Endpoint: DELETE /api/produtos/{id}
Descrição: Remove um produto do estoque.

## Buscar Produtos por Nome:
Endpoint: GET /api/produtos/buscar
Descrição: Retorna uma lista de produtos cujo nome contém a string fornecida como parâmetro.

# Linguagens e Tecnologias Utilizadas
- Java: A linguagem de programação principal usada para desenvolver a API.
- Spring Boot: Framework utilizado para simplificar a configuração e o desenvolvimento de aplicações Java.
- Spring Data JPA: Usado para facilitar a interação com o banco de dados.
- MySQL: Banco de dados relacional utilizado para armazenar os dados dos produtos.
- Maven: Ferramenta de gerenciamento de dependências e build utilizada no projeto.

```bash
## Estrutura do Projeto
Diretórios e Arquivos

│
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── example
│   │   │           └── estoqueapi
│   │   │               ├── controller
│   │   │               │   └── ProdutoController.java
│   │   │               ├── model
│   │   │               │   └── Produto.java
│   │   │               ├── repository
│   │   │               │   └── ProdutoRepository.java
│   │   │               ├── service
│   │   │               │   └── ProdutoService.java
│   │   │               └── EstoqueApiApplication.java
│   │   └── resources
│   │       ├── application.properties
│   │       └── static
│   │       └── templates
│   └── test
│       └── java
│           └── com
│               └── example
│                   └── estoqueapi
│                       └── EstoqueApiApplicationTests.java
│
└── pom.xml
```

## Descrição dos Arquivos
- EstoqueApiApplication.java: Classe principal que inicia a aplicação Spring Boot.
- controller/ProdutoController.java: Controlador que define os endpoints da API para operações CRUD.
- model/Produto.java: Classe modelo que representa a entidade Produto no banco de dados.
- repository/ProdutoRepository.java: Interface que estende JpaRepository para realizar operações de persistência no banco de dados.
- service/ProdutoService.java: Classe de serviço que contém a lógica de negócios e interage com o repositório.
- resources/application.properties: Arquivo de configuração que contém informações de conexão com o banco de dados e outras propriedades do Spring Boot.
- pom.xml: Arquivo de configuração do Maven que define as dependências e plugins necessários para o projeto.

# Resumo
Este projeto de API de controle de estoque em Spring Boot permite gerenciar produtos em um banco de dados MySQL, suportando operações CRUD e consultas personalizadas. Utiliza Java como linguagem principal, Spring Boot para a estrutura do backend, Spring Data JPA para persistência e MySQL como banco de dados relacional.
