# 📱 Agenda de Contatos

Projeto desenvolvido em **Java** para a disciplina de **Programação Orientada a Objetos (POO)**.

A aplicação é construída de forma incremental, evoluindo a estrutura de armazenamento de dados, as funcionalidades e a organização do código a cada nova versão.

---

## 🎯 Objetivo

Desenvolver um sistema de Agenda de Contatos em Java via console, aplicando na prática os conceitos fundamentais de programação, modularização e estruturas de dados estudados durante a disciplina.

---

## 📈 Evolução do Projeto

| Versão | Armazenamento / Estrutura | Principais Conceitos / Funcionalidades |
| :---: | :--- | :--- |
| `V.0.0.0` | Variáveis simples | Entrada e saída (`Scanner`), condicionais (`if-else`, `switch`) e repetição (`while`) |
| `V.0.1.0` | Arrays (Vetores) | Vetores, manipulação por índices, laço `for` e limitação de capacidade fixa |
| `V.0.2.0` | `List` / `ArrayList` | Coleções dinâmicas, métodos `add()`, `get()`, `remove()` e `size()` |
| `V.0.3.0` | `List` / `ArrayList` | Atualização de elementos com `set()` e implementação do CRUD completo |
| **`V.1.0.0`** | Modularização com Métodos | Refatoração em métodos estáticos (`public static void`), reuso de código e separação de responsabilidades |

---

## 🚀 Versão Atual — `V.1.0.0`

A versão **V.1.0.0** foca na **organização e modularização do código**. Todo o fluxo do programa, antes concentrado no método `main`, foi dividido em métodos específicos e bem definidos:

- **Controle da Aplicação:** `mostraInicializacao()`, `mostraMenu()`, `selecionaOpcao()` e `sair()`.
- **Operações do CRUD:**
  - `adicionar()` → Cadastro de novos contatos.
  - `listar()` → Exibição da lista completa.
  - `pesquisar()` → Busca por nome.
  - `atualizar()` → Edição de contatos existentes.
  - `excluir()` → Remoção de registros.

---

## ⚙️ Funcionalidades

1. ➕ **Adicionar contato:** Cadastra nome, celular e e-mail.
2. 📋 **Listar contatos:** Exibe todos os contatos cadastrados.
3. 🔎 **Procurar contato:** Busca um contato específico pelo nome.
4. ✏️ **Alterar contato:** Atualiza as informações de um contato existente.
5. 🗑️ **Excluir contato:** Remove um contato da agenda.
6. 🚪 **Sair:** Encerra a aplicação.

---

## 📂 Estrutura do Projeto

```text
Agenda-Contatos/
├── .gitignore
├── README.md
└── src/
    └── br/
        └── edu/
            └── principal/
                └── Principal.java
