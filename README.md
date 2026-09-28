# 📱 Agenda de Contatos

Projeto desenvolvido em **Java** para a disciplina de **Programação Orientada a Objetos (POO)**.

A aplicação é construída de forma incremental, evoluindo a estrutura de armazenamento de dados, as funcionalidades, a interface e a organização modular do código a cada nova versão.

---

## 🎯 Objetivo

Desenvolver um sistema de Agenda de Contatos em Java, aplicando na prática os conceitos fundamentais de programação, separação de responsabilidades em múltiplas classes, controle de fluxo e caixas de diálogo com `JOptionPane`.

---

## 📈 Evolução do Projeto

| Versão | Armazenamento / Estrutura | Principais Conceitos / Funcionalidades |
| :---: | :--- | :--- |
| `V.0.0.0` | Variáveis simples | Entrada/saída (`Scanner`), condicionais (`if-else`, `switch`) e repetição (`while`) |
| `V.0.1.0` | Arrays (Vetores) | Vetores, manipulação por índices, laço `for` e limitação de capacidade fixa |
| `V.0.2.0` | `List` / `ArrayList` | Coleções dinâmicas, métodos `add()`, `get()`, `remove()` e `size()` |
| `V.0.3.0` | `List` / `ArrayList` | Atualização de elementos com `set()` e implementação do CRUD completo |
| `V.1.0.0` | Modularização | Refatoração em métodos estáticos (`public static void`) na classe principal |
| `V.1.1.0` | Separação em Classes | Divisão em `Principal`, `Agenda` e `Uteis`, integração com `JOptionPane` e opção "Sobre" |
| **`V.1.1.1`** | Correção de Controle de Fluxo | Refatoração do método `sair()` retornando `boolean` para encerramento correto do `while` |

---

## 🚀 Versão Atual — `V.1.1.1`

A versão **V.1.1.1** traz um ajuste fino no controle de fluxo da aplicação e na passagem de parâmetros em Java:

- 🛑 **Ajuste na lógica de encerramento (`sair()`):** O método `sair()` na classe `Uteis` foi alterado de `void` para `boolean`, retornando `false`. Na classe `Principal`, o retorno passa a atualizar diretamente a variável `continuar = Uteis.sair()`, corrigindo o problema de passagem de parâmetro por valor e garantindo que o laço `while` seja encerrado corretamente.
- 📌 **Atualização de versão:** O banner inicial exibido ao executar a aplicação foi atualizado para **v1.1.1**.

---

## ⚙️ Funcionalidades

1. ➕ **Adicionar contato:** Cadastra nome, celular e e-mail.
2. 📋 **Listar contatos:** Exibe todos os contatos cadastrados no console.
3. 🔎 **Procurar contato:** Busca um contato específico pelo nome.
4. ✏️ **Alterar contato:** Atualiza as informações de um contato existente.
5. 🗑️ **Excluir contato:** Remove um contato da agenda.
6. 🚪 **Sair:** Encerra a execução da aplicação de forma segura.
7. ℹ️ **Sobre:** Exibe uma janela gráfica (`JOptionPane`) com dados do desenvolvedor.

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
                ├── Agenda.java
                ├── Principal.java
                └── Uteis.java
