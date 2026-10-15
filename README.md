# API Inteligente com Spring Boot

## Sobre o projeto

Este projeto foi desenvolvido como parte dos meus estudos na DIO. O objetivo é praticar Java, Spring Boot, criação de APIs REST e armazenamento de dados.

A aplicação permite cadastrar despesas, listar os registros e calcular o valor total das despesas.

## Tecnologias utilizadas

- Java 21
- Spring Boot
- Spring Data JPA
- Banco de dados H2
- Maven
- API REST

## Funcionalidades

- Cadastrar despesas.
- Listar despesas cadastradas.
- Calcular o total das despesas.
- Consultar o total por meio de endpoints.
- Armazenar os dados no banco H2.

## Endpoints

| Método | Endpoint | Descrição |
|---|---|---|
| GET | `/` | Página inicial |
| GET | `/teste` | Testar a API |
| POST | `/despesas` | Cadastrar despesa |
| GET | `/despesas` | Listar despesas |
| GET | `/despesas/total` | Calcular o total |
| GET | `/comando?texto=total` | Consultar total por comando |
| GET | `/comando/total` | Consultar total |

## Exemplo de cadastro

Envie uma requisição POST para `/despesas` com este JSON:

```json
{
  "descricao": "Internet",
  "valor": 100.00
}
```

## Como executar

1. Instale o Java 21.
2. Abra o terminal na pasta do projeto.
3. Execute:

```powershell
.\mvnw.cmd spring-boot:run
```

4. Acesse `http://localhost:8080/teste` no navegador.

## Aprendizados

Neste projeto, pratiquei a criação de endpoints REST, a organização do código em controller e service, a persistência de dados com Spring Data JPA e o cálculo de despesas.

## Autora

Projeto desenvolvido para fins de estudo na DIO.