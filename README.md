# Restaurant Menu

![Java](https://img.shields.io/badge/Java-17-%23ED8B00?style=flat-square&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3-%236DB33F?style=flat-square&logo=spring)
![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

Aplicação full-stack para gerenciamento de cardápios digitais com painel administrativo e API REST.


## Visão Geral

O projeto permite cadastrar, editar, remover e visualizar itens do cardápio por meio de uma interface web integrada a uma API REST.

A aplicação foi desenvolvida utilizando arquitetura desacoplada entre frontend e backend, com persistência em banco relacional e execução via containers Docker.

## Funcionalidades

- Gerenciamento de itens do cardápio
- Cadastro, edição e exclusão (CRUD)
- Painel administrativo
- API REST documentada
- Interface responsiva
- Execução containerizada

---

## Capturas de Tela

<table align="center">
<tr>

<td align="center">

**Página Inicial**

<img src="docs/home-desktop.png" width="420"/>

</td>

<td align="center">

**Painel Administrativo**

<img src="docs/medium-adminpanel.png" width="420"/>

</td>

</tr>

<tr>

<td align="center">

**Adicionar Item**

<img src="docs/adminpanel-add.png" width="420"/>

</td>

<td align="center">

**Editar Item**

<img src="docs/adminpanel-update.png" width="420"/>

</td>

</tr>
</table>

---

## Arquitetura

```mermaid
flowchart LR

A[React]
--> B[Spring Boot]
--> C[MySQL]
```

---

## Stack Tecnológica

| Camada | Tecnologia |
|---|---|
| Backend | Spring Boot + JPA |
| Frontend | React |
| Banco de Dados | MySQL |
| Documentação | OpenAPI / Swagger |
| Testes | JUnit |
| Infraestrutura | Docker |

---

## Documentação da API

Swagger disponível em:

```txt
http://localhost:8080/swagger-ui.html
```

<img src="docs/swagger-endpoints.png" width="900"/>

---

## Executando o Projeto

### Pré-requisitos

- Docker

### Inicialização

```bash
docker compose up --build
```

---

## Serviços

| Serviço | URL |
|---|---|
| Frontend | http://localhost |
| Backend | http://localhost:8080 |
| Swagger | http://localhost:8080/swagger-ui.html |

---

## Roadmap

- [x] CRUD de cardápio
- [x] Painel administrativo
- [x] API documentada
- [ ] Autenticação
- [ ] Upload de imagens
- [ ] Deploy automatizado

---

## Licença

Distribuído sob licença MIT.
