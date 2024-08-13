Aqui está o `README.md` personalizado para o repositório `product-API`:

```markdown
# Product API

Uma API RESTful para gerenciamento de produtos, desenvolvida com Spring Boot e Java 21.

## Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Instalação e Execução](#instalação-e-execução)
- [Documentação da API](#documentação-da-api)
- [Testes](#testes)
- [Contribuindo](#contribuindo)
- [Licença](#licença)

## Sobre o Projeto

A Product API é uma aplicação que permite gerenciar informações de produtos, incluindo a criação, visualização, atualização e exclusão de produtos. Este projeto é um exemplo de aplicação backend usando Spring Boot, que pode ser usado para estudos ou como base para outros projetos.

## Tecnologias Utilizadas

- **Java 21**: Linguagem de programação utilizada.
- **Spring Boot 3.3.2**: Framework para construção da API.
- **Maven 3.9.8**: Ferramenta de automação de compilação e gerenciamento de dependências.
- **Docker**: Para containerização da aplicação.

## Instalação e Execução

### Pré-requisitos

Antes de iniciar, certifique-se de ter instalado:

- [Java 21](https://www.oracle.com/java/technologies/javase/jdk21-archive-downloads.html)
- [Maven](https://maven.apache.org/download.cgi)
- [Docker](https://www.docker.com/) (opcional)

### Passos para Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/pdrotmz/product-API.git
   cd product-API
   ```

2. Compile e execute a aplicação:

   - **Com Maven:**
     ```bash
     mvn clean install
     mvn spring-boot:run
     ```

   - **Com Docker:**
     ```bash
     docker build -t product-api .
     docker run -p 8080:8080 product-api
     ```

A aplicação estará disponível em `https://product-api-jkqt.onrender.com`.

## Documentação da API

### Endpoints Principais

- **GET /products**: Retorna uma lista de todos os produtos.
- **GET /products/{id}**: Retorna os detalhes de um produto específico.
- **POST /product**: Cria um novo produto.
- **PUT /products/{id}**: Atualiza as informações de um produto existente.
- **DELETE /products/{id}**: Remove um produto pelo ID.

### Exemplo de Requisição - Criar Produto

```bash
curl -X POST http://localhost:8080/products \
-H "Content-Type: application/json" \
-d '{
  "name": "Novo Produto",
  "value" : 49.99,
}'
```

### Exemplo de Resposta - Listar Produtos

```json
[
  {
    "idProduct": "value",
    "name": "Produto Exemplo",
    "value": 19.99,
  },
  {
    "idProduct": "value",
    "name": "Outro Produto",
    "price": 29.99,
  }
]
```

## Testes

Para executar os testes automatizados:

```bash
mvn test
```

Para construir o projeto sem executar os testes:

```bash
mvn clean install -DskipTests
```

## Contribuindo

Contribuições são bem-vindas! Siga os passos abaixo para contribuir:

1. Faça um fork do projeto.
2. Crie uma nova branch para sua feature (`git checkout -b feature/nova-feature`).
3. Faça commit das suas alterações (`git commit -m 'Adiciona nova feature'`).
4. Faça push para a branch (`git push origin feature/nova-feature`).
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
```

Esse `README.md` é completo e adaptado especificamente para o repositório `product-API`, fornecendo todas as informações necessárias para configuração, uso, testes e contribuição.
