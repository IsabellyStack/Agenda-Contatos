# 📱 Agenda de Contatos

Projeto desenvolvido em **Java** na disciplina de **Programação Orientada a Objetos (POO)**.

A aplicação é desenvolvida de forma incremental, evoluindo a estrutura de armazenamento e as funcionalidades a cada versão.

## 🎯 Objetivo

Desenvolver uma Agenda de Contatos aplicando os conceitos estudados durante a disciplina.

## 📈 Evolução

| Versão | Armazenamento | Principais conceitos |
|---|---|---|
| `V.0.0.0` | Variáveis simples | `String`, `Scanner`, `if-else`, `switch` e `while` |
| `V.0.1.0` | Arrays | Vetores, índices, `for` e capacidade fixa |
| `V.0.2.0` | `List` + `ArrayList` | Tamanho dinâmico, `add()`, `get()`, `remove()` e `size()` |
| `V.0.3.0` | `List` + `ArrayList` | Alteração de contatos com `set()` e CRUD |

### V.0.3.0 — Versão atual

A versão atual adiciona a funcionalidade de **alterar contatos** utilizando `set()`.

O sistema passa a possuir um CRUD completo:

- **CREATE** → Adicionar
- **READ** → Listar e procurar
- **UPDATE** → Alterar
- **DELETE** → Excluir

## ⚙️ Funcionalidades

- ➕ Adicionar contato
- 📋 Listar contatos
- 🔎 Procurar contato
- ✏️ Alterar contato
- 🗑️ Excluir contato
- 🚪 Sair

## 📂 Estrutura do projeto

```text
Agenda-Contatos/
├── .gitignore
├── README.md
└── src/
    └── br/
        └── edu/
            └── principal/
                └── Principal.java
