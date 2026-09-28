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
| **`V.2.1.0`** | Persistência em Arquivo (`.txt`) | Implementação da classe `Persistencia` (`FileWriter`, `PrintWriter`, `BufferedReader`), salvando e carregando dados automaticamente |

---

## 🚀 Versão Atual — `V.2.1.0`

A versão **V.2.1.0** introduz a persistência de dados em arquivo texto (`contatos.txt`), permitindo que as informações cadastradas permaneçam gravadas mesmo após o encerramento da aplicação:

- 💾 **Persistência de Dados (`Persistencia.java`):**
  - **`carregarContatos()`:** Ao iniciar o programa, lê o arquivo `contatos.txt` utilizando `BufferedReader` e `FileReader`, reconstruindo as listas dinâmicas na memória. Trata registros malformados e arquivos inexistentes.
  - **`salvarContatos()`:** Ao selecionar a opção de encerramento, grava todos os contatos no arquivo `contatos.txt` formatados com separador ponto e vírgula (`;`) através de `FileWriter` e `PrintWriter`.
- 🔄 **Integração com o Fluxo Principal:** A inicialização do sistema carrega automaticamente os dados salvos anteriormente, e a opção 6 ("Sair") salva o estado atual antes de encerrar o programa.
- 📌 **Atualização de versão:** Banner inicial atualizado para a versão **v2.1.0**.

---

## ⚙️ Funcionalidades

1. ➕ **Adicionar contato:** Cadastra nome, celular e e-mail em memória.
2. 📋 **Listar contatos:** Exibe todos os contatos cadastrados no console.
3. 🔎 **Procurar contato:** Busca um contato específico pelo nome.
4. ✏️ **Alterar contato:** Atualiza as informações de um contato existente.
5. 🗑️ **Excluir contato:** Remove um contato da agenda.
6. 🚪 **Sair:** Salva os dados em `contatos.txt` e encerra a execução da aplicação.
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
                ├── Persistencia.java
                ├── Principal.java
                └── Uteis.java
