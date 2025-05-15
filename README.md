# Catálogo de Produtos

Este projeto é um sistema web para gerenciar um catálogo de produtos, permitindo o cadastro, aplicação de descontos e envio de notificações. O sistema simula uma loja ou um sistema interno de gestão.

## Objetivos

- Cadastrar produtos
- Listar produtos
- Aplicar diferentes estratégias de desconto
- Notificar automaticamente os usuários quando um novo produto é cadastrado

## Tecnologias Utilizadas

- Java 17+
- Spring Boot
- Spring Web
- Spring Data JPA
- H2 ou PostgreSQL
- Lombok
- MapStruct (opcional para conversões DTO)

## Estrutura do Projeto

```
src
├── main
│   ├── java
│   │   └── com
│   │       └── seuprojeto
│   │           ├── controller        # Controladores para gerenciar requisições HTTP
│   │           ├── service           # Classes de serviço com lógica de negócios
│   │           ├── model             # Classes de modelo representando a estrutura de dados
│   │           ├── repository         # Interfaces de repositório para acesso a dados
│   │           ├── dto               # Objetos de Transferência de Dados (DTOs)
│   │           ├── strategy          # Implementação do Padrão Strategy para descontos
│   │           ├── observer          # Implementação do Padrão Observer para notificações
│   │           ├── factory           # Implementação do Padrão Factory Method para criadores de notificadores
│   │           ├── decorator         # Implementação do Padrão Decorator para funcionalidades extras
│   │           └── config            # Classes de configuração do Spring
│   └── resources
│       ├── application.properties     # Configurações do aplicativo Spring Boot
│       └── data.sql                  # Scripts SQL para inicialização do banco de dados
└── test
    └── java
        └── com
            └── seuprojeto
                └── service           # Testes de unidade e integração para a camada de serviço
```

## Como Executar o Projeto

1. Clone o repositório:
   ```
   git clone <URL_DO_REPOSITORIO>
   ```

2. Navegue até o diretório do projeto:
   ```
   cd catalogo-produtos
   ```

3. Execute o projeto com Maven:
   ```
   mvn spring-boot:run
   ```

4. Acesse a aplicação em `http://localhost:8080`.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.