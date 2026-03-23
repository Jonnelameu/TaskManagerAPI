# TaskManagerAPI

 Task Manager API

API REST para gerenciamento de tarefas desenvolvida com **ASP.NET Core**, **Entity Framework Core** e **SQL Server**.

Projeto criado com objetivo de aprendizado em **desenvolvimento Full Stack** e preparação para vagas de **estágio ou desenvolvedor júnior**.

---

 Tecnologias

* C#
* ASP.NET Core Web API
* Entity Framework Core
* SQL Server
* REST API
* JSON

---

 Funcionalidades

* Criar tarefas
* Listar tarefas
* Atualizar tarefas
* Deletar tarefas

Este projeto implementa um **CRUD completo**.

---

 Estrutura do Projeto

```
TaskManagerAPI
│
├── Controllers
├── Models
├── Data
├── Services
├── Program.cs
└── appsettings.json
```

---

 Endpoints

## Listar tarefas

```
GET /api/tasks
```

## Criar tarefa

```
POST /api/tasks
```

Body:

```json
{
  "title": "Nova tarefa",
  "done": false
}
```

## Atualizar tarefa

```
PUT /api/tasks/{id}
```

## Deletar tarefa

```
DELETE /api/tasks/{id}
```

---

 Como executar

1. Abrir o projeto no **Visual Studio**
2. Configurar a string de conexão no `appsettings.json`
3. Executar as migrations:

```
Add-Migration InitialCreate
Update-Database
```

4. Rodar o projeto (F5)

A API estará disponível em:

```
https://localhost:xxxx/api/tasks
```

---

 Objetivo do Projeto

Este projeto foi desenvolvido para praticar:

* criação de APIs REST
* conexão com banco de dados
* organização profissional de código
* uso de Entity Framework Core
