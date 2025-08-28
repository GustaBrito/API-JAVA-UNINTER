# 📋 API de Gerenciamento de Tarefas

Uma API RESTful completa para gerenciamento de tarefas, desenvolvida em Java com Spring Boot.

![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.5.5-green.svg) _ 
![Java](https://img.shields.io/badge/Java-21-blue.svg) _ 
![License](https://img.shields.io/badge/License-MIT-yellow.svg) _ 

## 🚀 Tecnologias Utilizadas

- **Java 21**
- **Spring Boot 3.5.5**
- **Spring Data JPA**
- **H2 Database** (em memória)
- **Maven**
- **Postman** para testes

## 📋 Funcionalidades

| Funcionalidade | Método HTTP | Endpoint |
|----------------|-------------|----------|
| ✅ Criar tarefa | `POST` | `/api/tarefas` |
| ✅ Listar todas as tarefas | `GET` | `/api/tarefas` |
| ✅ Buscar tarefa por ID | `GET` | `/api/tarefas/{id}` |
| ✅ Atualizar tarefa | `PUT` | `/api/tarefas/{id}` |
| ✅ Excluir tarefa | `DELETE` | `/api/tarefas/{id}` |

## 🏗️ Estrutura do Projeto

```texto
src/
├── main/
│   ├── java/com/exemplo/api_tarefas/
│   │   ├── model/Tarefa.java          # Entidade JPA
│   │   ├── repository/TarefaRepository.java  # Interface JpaRepository
│   │   ├── controller/TarefaController.java  # Endpoints REST
│   │   └── ApiTarefasApplication.java # Classe principal
│   └── resources/
│       └── application.properties     # Configurações
```

## 📝 Modelo de Dados

```java
public class Tarefa {
    private Long id;                    // ID automático
    private String nome;                // Nome da tarefa (100 chars)
    private LocalDate dataEntrega;      // Data de entrega
    private String responsavel;         // Responsável (100 chars)
}
```

## 📊 Status Codes
| Status | Code |	Descrição |
|--------|------|-----------|
| 200 | OK |	Requisição bem-sucedida | 
| 201 | Created |	Recurso criado com sucesso | 
| 204 | No Content |	Exclusão bem-sucedida | 
| 404 | Not Found |	Recurso não encontrado | 

---

🎯 Projeto desenvolvido para a disciplina de Desenvolvimento Web Back end

---
