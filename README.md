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
| `V.3.0.0` | Classes e Objetos | Modulo de POO com a criação da classe `Contato` (atributos, construtores e getters/setters) |
| **`V.3.1.0`** | **Coleção de Objetos** | **Gerenciamento de instâncias com `List<Contato>` (`ArrayList`), combinando POO com coleções dinâmicas** |

---

## 🚀 Versão Atual — `V.3.1.0`

A versão **V.3.1.0** consolida o uso de **Programação Orientada a Objetos (POO)** integrada a **Coleções Dinâmicas**:

- 🧩 **Molde e Objeto (`Contato.java`):** Abstração do contato em uma classe com atributos encapsulados (`nome`, `celular`, `email`), construtores customizados, métodos acessores (*getters/setters*) e sobrita do `toString()`.
- 📦 **Coleção Tipada (`List<Contato>`):** A classe `Agenda` deixa de gerenciar listas de strings separadas e passa a manipular uma única coleção de objetos `Contato` (`List<Contato>`), garantindo type safety e código mais limpo.
- 💾 **Persistência de Objetos (`Persistencia.java`):** Leitura do arquivo `contatos.txt` instanciando objetos `Contato` diretamente na memória e conversão da lista de objetos para o arquivo no salvamento.
- 📌 **Atualização de versão:** Banner inicial atualizado para a versão **v3.1.0**.

---

## ⚙️ Funcionalidades

1. ➕ **Adicionar contato:** Cria e insere um novo objeto `Contato` na lista.
2. 📋 **Listar contatos:** Percorre a lista de objetos exibindo as informações formatadas no console.
3. 🔎 **Procurar contato:** Realiza busca por nome filtrando na coleção de objetos `Contato`.
4. ✏️ **Alterar contato:** Atualiza os atributos do objeto selecionado na lista.
5. 🗑️ **Excluir contato:** Remove o objeto `Contato` da lista.
6. 🚪 **Sair:** Grava todos os objetos da lista em `contatos.txt` e encerra a aplicação.
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
