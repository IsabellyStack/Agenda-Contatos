# 📱 Agenda de Contatos

Projeto desenvolvido em **Java** para a disciplina de **Programação Orientada a Objetos (POO)**.

A aplicação é construída de forma incremental, evoluindo a estrutura de armazenamento de dados, as funcionalidades, a interface e a organização modular do código a cada nova versão.

---

## 🎯 Objetivo

Desenvolver um sistema de Agenda de Contatos em Java, aplicando na prática os conceitos fundamentais de programação, separação de responsabilidades em múltiplas classes, controle de fluxo, caixas de diálogo com `JOptionPane` e persistência de dados em arquivos de texto.

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
| `V.1.1.1` | Correção de Controle de Fluxo | Refatoração do método `sair()` retornando `boolean` para encerramento correto do `while` |
| `V.2.1.0` | Persistência em Arquivo (`.txt`) | Implementação da classe `Persistencia` (`FileWriter`, `PrintWriter`, `BufferedReader`), salvando e carregando dados automaticamente |
| `V.3.0.0` | Classe e Objetos | Introdução à Programação Orientada a Objetos com a criação da classe `Contato` |
| **`V.3.2.0`** | **CRUD Orientado a Objetos** | **Adaptação das operações CRUD e da persistência para utilizar `List<Contato>`** |

---

## 🚀 Versão Atual — `V.3.2.0`

A versão **V.3.2.0** consolida o refatoramento completo do sistema para **Programação Orientada a Objetos (POO)**:

- 🧱 **Abstração e Encapsulamento (`Contato.java`):** Utilização da classe `Contato` com atributos privados (`nome`, `celular`, `email`), construtores e métodos *getters/setters*.
- 🔄 **CRUD Refatorado (`Agenda.java`):** Todas as operações de cadastro, listagem, busca, alteração e remoção agora manipulam diretamente uma única coleção de objetos (`List<Contato>`), eliminando o uso de múltiplas listas paralelas.
- 💾 **Persistência Adaptada (`Persistencia.java`):** O processo de leitura e gravação no arquivo `contatos.txt` foi reconstruído para instanciar e serializar objetos `Contato` diretamente na memória.
- 📌 **Atualização de versão:** Banner inicial atualizado para a versão **v3.2.0**.

---

## ⚙️ Funcionalidades

1. ➕ **Adicionar contato:** Cria e cadastra uma nova instância da classe `Contato` na lista.
2. 📋 **Listar contatos:** Exibe todos os objetos `Contato` cadastrados consultando seus atributos.
3. 🔎 **Procurar contato:** Realiza a busca por nome diretamente nos objetos da lista.
4. ✏️ **Alterar contato:** Atualiza os atributos do objeto `Contato` selecionado via *setters*.
5. 🗑️ **Excluir contato:** Remove o objeto `Contato` da coleção.
6. 🚪 **Sair:** Grava todos os objetos salvos na `List<Contato>` dentro do arquivo `contatos.txt` e encerra a aplicação.
7. ℹ️ **Sobre:** Exibe uma janela gráfica (`JOptionPane`) com dados do desenvolvedor.

---

## 📂 Estrutura do Projeto

```text
Agenda-Contatos/
├── .gitignore
├── README.md
├── contatos.txt
└── src/
    └── br/
        └── edu/
            └── principal/
                ├── Agenda.java
                ├── Contato.java
                ├── Persistencia.java
                ├── Principal.java
                └── Uteis.java
