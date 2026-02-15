# FórumHub — Desafio Alura (Oracle ONE)

Este repositório contém o projeto **FórumHub**, desenvolvido como parte do **Desafio da Alura em parceria com o Oracle ONE**, com foco na criação de um back-end para um fórum de tópicos e respostas.

A ideia é oferecer uma API organizada e segura para criação, consulta, atualização e exclusão de tópicos, seguindo boas práticas e regras de negócio do desafio.

---

## ✨ O que já foi implementado

- CRUD de **Tópicos** (criar, listar com paginação, detalhar, atualizar e excluir)
- Validações de campos e regras de negócio (ex.: campos obrigatórios e prevenção de duplicidade)
- Autenticação com **login** e geração de **token JWT**
- Proteção das rotas com **Spring Security** (Bearer Token)

---

## 🧰 Tecnologias utilizadas

- **Java 21**
- **Spring Boot**
- **Spring Web**
- **Spring Data JPA (Hibernate)**
- **MySQL**
- **Flyway** (migrations do banco)
- **Spring Security**
- **JWT (JSON Web Token)** para autenticação via Bearer Token
- **Lombok** para reduzir boilerplate
- **Bean Validation** (`@Valid`, `@NotBlank`, `@NotNull`)

---

## 🚀 Como a API funciona (visão geral)

1. O usuário faz login em `/login` com email e senha
2. A API retorna um token JWT
3. Esse token deve ser enviado nas próximas requisições no header:

`Authorization: Bearer SEU_TOKEN_AQUI`

---

## 🔮 Próximos passos / melhorias futuras

Este projeto ainda pode evoluir bastante. Próximas atualizações devem incluir:

- Mais endpoints para trabalhar com outras entidades do sistema (ex.: **Respostas**, **Usuários**, **Perfis** e **Cursos**)
- Regras de autorização mais detalhadas (ex.: permissões por perfil)
- Uma interface simples (front-end) para consumir a API e facilitar o uso do fórum

---

## 📌 Observações

Projeto desenvolvido como estudo e prática, priorizando organização, legibilidade e evolução incremental conforme as etapas do desafio.
