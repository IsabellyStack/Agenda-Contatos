# 📱 Agenda de Contatos

Projeto desenvolvido em **Java** para a disciplina de **Programação Orientada a Objetos (POO)**.

A aplicação é construída de forma incremental, evoluindo a estrutura de armazenamento de dados, as funcionalidades, a interface e a organização modular do código a cada nova versão.

---

## 🎯 Objetivo

Desenvolver um sistema de Agenda de Contatos em Java, aplicando na prática os conceitos fundamentais de programação, separação de responsabilidades em múltiplas classes, interface via console e caixas de diálogo do `JOptionPane`.

---

## 📈 Evolução do Projeto

| Versão | Armazenamento / Estrutura | Principais Conceitos / Funcionalidades |
| :---: | :--- | :--- |
| `V.0.0.0` | Variáveis simples | Entrada/saída (`Scanner`), condicionais (`if-else`, `switch`) e repetição (`while`) |
| `V.0.1.0` | Arrays (Vetores) | Vetores, manipulação por índices, laço `for` e limitação de capacidade fixa |
| `V.0.2.0` | `List` / `ArrayList` | Coleções dinâmicas, métodos `add()`, `get()`, `remove()` e `size()` |
| `V.0.3.0` | `List` / `ArrayList` | Atualização de elementos com `set()` e implementação do CRUD completo |
| `V.1.0.0` | Modularização com Métodos | Refatoração em métodos estáticos (`public static void`) na classe principal |
| **`V.1.1.0`** | Separação em Múltiplas Classes | Organização modular em `Principal`, `Agenda` e `Uteis`, integração com `JOptionPane` e opção "Sobre" |

---

## 🚀 Versão Atual — `V.1.1.0`

A versão **V.1.1.0** avança na **arquitetura do código**, dividindo as responsabilidades da aplicação entre classes específicas:

- 🚀 **`Principal.java`**: Ponto de entrada do sistema. Responsável apenas por instanciar as coleções de dados, controlar o laço de repetição (`while`) e direcionar as opções escolhidas no menu via `switch`.
- 📂 **`Agenda.java`**: Concentra a lógica das operações do **CRUD** (`adicionar`, `listar`, `pesquisar`, `atualizar` e `excluir`).
- 🛠️ **`Uteis.java`**: Agrupa funções utilitárias do sistema, como exibição da mensagem inicial, montagem do menu, leitura de opções, encerramento e exibição da janela "Sobre".
- 💬 **`JOptionPane`**: Introduz o uso de componentes gráficos (`javax.swing.JOptionPane`) para exibir informações sobre a autoria do projeto.

---

## ⚙️ Funcionalidades

1. ➕ **Adicionar contato:** Cadastra nome, celular e e-mail.
2. 📋 **Listar contatos:** Exibe todos os contatos cadastrados no console.
3. 🔎 **Procurar contato:** Busca um contato específico pelo nome.
4. ✏️ **Alterar contato:** Atualiza as informações de um contato existente.
5. 🗑️ **Excluir contato:** Remove um contato da agenda.
6. 🚪 **Sair:** Encerra a execução da aplicação.
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
                └── Uteis.java# 📱 Agenda de Contatos

Projeto desenvolvido em **Java** para a disciplina de **Programação Orientada a Objetos (POO)**.

A aplicação é construída de forma incremental, evoluindo a estrutura de armazenamento de dados, as funcionalidades, a interface e a organização modular do código a cada nova versão.

---

## 🎯 Objetivo

Desenvolver um sistema de Agenda de Contatos em Java, aplicando na prática os conceitos fundamentais de programação, separação de responsabilidades em múltiplas classes, interface com console e caixas de diálogo do `JOptionPane`.

---

## 📈 Evolução do Projeto

| Versão | Armazenamento / Estrutura | Principais Conceitos / Funcionalidades |
| :---: | :--- | :--- |
| `V.0.0.0` | Variáveis simples | Entrada/saída (`Scanner`), condicionais (`if-else`, `switch`) e repetição (`while`) |
| `V.0.1.0` | Arrays (Vetores) | Vetores, manipulação por índices, laço `for` e limitação de capacidade fixa |
| `V.0.2.0` | `List` / `ArrayList` | Coleções dinâmicas, métodos `add()`, `get()`, `remove()` e `size()` |
| `V.0.3.0` | `List` / `ArrayList` | Atualização de elementos com `set()` e implementação do CRUD completo |
| `V.1.0.0` | Modularização com Métodos | Refatoração em métodos estáticos (`public static void`) na classe principal |
| **`V.1.1.0`** | Separação em Múltiplas Classes | Organização modular em `Agenda` e `Uteis`, integração com `JOptionPane` e opção "Sobre" |

---

## 🚀 Versão Atual — `V.1.1.0`

A versão **V.1.1.0** avança na **arquitetura do código**, dividindo as responsabilidades da aplicação em arquivos/classes dedicados:

- 📂 **`Agenda.java`**: Concentra toda a lógica das operações do **CRUD** (`adicionar`, `listar`, `pesquisar`, `atualizar` e `excluir`).
- 🛠️ **`Uteis.java`**: Gerencia funções utilitárias do sistema, como renderização do menu, leitura de opções, mensagem inicial, encerramento e exibição da janela "Sobre".
- 💬 **`JOptionPane`**: Introduz o uso do componente gráfico do Swing para exibir a caixa de diálogo com as informações de autoria do projeto.
- ℹ️ **Opção 7 ("Sobre")**: Nova funcionalidade no menu principal que exibe os dados do desenvolvedor.

---

## ⚙️ Funcionalidades

1. ➕ **Adicionar contato:** Cadastra nome, celular e e-mail.
2. 📋 **Listar contatos:** Exibe todos os contatos cadastrados no console.
3. 🔎 **Procurar contato:** Busca um contato específico pelo nome.
4. ✏️ **Alterar contato:** Atualiza as informações de um contato existente.
5. 🗑️ **Excluir contato:** Remove um contato da agenda.
6. 🚪 **Sair:** Encerra a execução da aplicação.
7. ℹ️ **Sobre:** Exibe uma janela gráfica (`JOptionPane`) com informações sobre o desenvolvedor do projeto.

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
