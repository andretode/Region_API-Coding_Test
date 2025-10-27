# Avaliação – Desenvolvedor Web (Estágio)

Este projeto tem como objetivo avaliar conhecimentos práticos em **desenvolvimento backend com .NET 8** e **integração com banco de dados PostgreSQL**, por meio da implementação de uma **API REST**.

---

## 🎯 Desafio

Implementar uma **API** que disponibilize **endpoints para CRUD de regiões**.

Uma **região** é uma entidade composta pelos seguintes campos:

- **UF** – Unidade Federativa (Estado)
- **Região** – Cidade
- **Situação** – Indica se a região está ativa ou inativa

O frontend (não incluso nesta avaliação) irá consumir esta API para exibir, criar e gerenciar as regiões.

---

## 🧩 Endpoints Requeridos

| Método | Endpoint | Descrição |
|--------|-----------|-----------|
| `GET` | `/regioes` | Retorna uma lista de todas as regiões existentes |
| `GET` | `/regioes/{id}` | Retorna uma região específica pelo seu ID |
| `POST` | `/regioes` | Cria uma nova região |
| `PUT` | `/regioes` | Atualiza uma região existente |
| `PATCH` | `/regioes/{id}` | Ativa ou desativa uma região existente |

---

## ⚙️ Regras de Negócio

- Todos os campos são **obrigatórios** ao criar uma nova região.
- **Não pode existir** mais de uma região com o **mesmo nome** para o **mesmo estado (UF)**, mesmo que inativa.
- A **inativação** de uma região deve ser **lógica**, ou seja, **não excluir fisicamente** o registro no banco.

---

## 🛠️ Tecnologias e Padrões

- **.NET 8 (C#)**
- **PostgreSQL**
- Arquitetura limpa e boas práticas de desenvolvimento são bem-vindas.
- Implementar versionamento de API, DTOs e tratamento de erros será considerado um diferencial.

---

## 🚀 Sugestões de Implementação

- Usar **Entity Framework Core** para o mapeamento e persistência dos dados.
- Utilizar **Migrations** para criação do schema no banco de dados.
- Retornar códigos HTTP adequados (`201`, `400`, `404`, `409`, etc.).
- Implementar **Swagger** para documentação dos endpoints.

---

## 🧪 Critérios de Avaliação

- Clareza e organização do código
- Cumprimento dos requisitos funcionais
- Aderência às boas práticas da linguagem e framework
- Estrutura e legibilidade da API
- Uso correto do versionamento e tratamento de erros

---

## 📦 Como enviar o projeto?

Crie um projeto no **seu perfil do GitHub** para ir commitando a evolução do seu código.

Ao final, favor enviar o link do projeto GitHub para andre@adaptum.com.br.
