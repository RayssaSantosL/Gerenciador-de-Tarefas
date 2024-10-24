# Gerenciador-de-Tarefas
Gerenciador de tarefas (To-Do List em Java)

# Documentação do Projeto: Gerenciador de Tarefas

## Sumário

1. [Descrição do Projeto](#descrição-do-projeto)
2. [Requisitos](#requisitos)
3. [Estrutura do Projeto](#estrutura-do-projeto)
4. [Classes e Métodos](#classes-e-métodos)
5. [Uso](#uso)
6. [Possíveis Melhorias](#possíveis-melhorias)

## Descrição do Projeto

O Gerenciador de Tarefas é uma aplicação em Java que permite aos usuários adicionar, listar, marcar como concluídas e remover tarefas de uma lista. O objetivo é fornecer uma interface simples para gerenciar atividades diárias.

## Requisitos

- **Java Development Kit (JDK)**: Versão 8 ou superior.
- **Ambiente de Desenvolvimento**: IDE como Eclipse, IntelliJ IDEA, ou qualquer editor de texto que suporte Java.
- **Sistema Operacional**: Qualquer sistema que suporte Java.

## Estrutura do Projeto

O projeto é dividido em três classes principais:

1. `Tarefa`
2. `GerenciadorDeTarefas`
3. `Main`

### Estrutura de Diretórios

```
/GerenciadorDeTarefas
│
├── Tarefa.java
├── GerenciadorDeTarefas.java
└── Main.java
```

## Classes e Métodos

### 1. Classe `Tarefa`

A classe `Tarefa` representa uma tarefa individual.

#### Atributos:

- `String descricao`: Descrição da tarefa.
- `boolean concluida`: Indica se a tarefa foi concluída.

#### Métodos:

- **Construtor**: `public Tarefa(String descricao)`
  - Inicializa a tarefa com uma descrição e a marca como não concluída.

- **getDescricao()**: `public String getDescricao()`
  - Retorna a descrição da tarefa.

- **isConcluida()**: `public boolean isConcluida()`
  - Retorna se a tarefa está concluída.

- **marcarComoConcluida()**: `public void marcarComoConcluida()`
  - Marca a tarefa como concluída.

- **toString()**: `public String toString()`
  - Retorna uma representação textual da tarefa, indicando se está concluída ou não.

### 2. Classe `GerenciadorDeTarefas`

A classe `GerenciadorDeTarefas` gerencia uma lista de tarefas.

#### Atributos:

- `List<Tarefa> tarefas`: Lista que armazena as tarefas.

#### Métodos:

- **Construtor**: `public GerenciadorDeTarefas()`
  - Inicializa a lista de tarefas.

- **adicionarTarefa(String descricao)**: `public void adicionarTarefa(String descricao)`
  - Adiciona uma nova tarefa à lista.

- **listarTarefas()**: `public void listarTarefas()`
  - Lista todas as tarefas com suas descrições e status.

- **marcarTarefaComoConcluida(int indice)**: `public void marcarTarefaComoConcluida(int indice)`
  - Marca a tarefa no índice especificado como concluída.

- **removerTarefa(int indice)**: `public void removerTarefa(int indice)`
  - Remove a tarefa no índice especificado da lista.

### 3. Classe `Main`

A classe `Main` é o ponto de entrada da aplicação.

#### Métodos:

- **main(String[] args)**: `public static void main(String[] args)`
  - Interage com o usuário através do console, oferecendo opções para gerenciar tarefas.

## Uso

1. Compile o projeto utilizando o JDK.
2. Execute a classe `Main`.
3. Siga as instruções no console para adicionar, listar, marcar ou remover tarefas.
4. Escolha a opção "0" para sair do aplicativo.

## Possíveis Melhorias

- **Persistência de Dados**: Implementar a funcionalidade para salvar e carregar tarefas de um arquivo.
- **Interface Gráfica**: Criar uma interface gráfica utilizando JavaFX ou Swing.
- **Prioridade das Tarefas**: Adicionar um sistema de priorização para as tarefas.
- **Categorias**: Permitir que o usuário categorize as tarefas.
- **Data de Vencimento**: Adicionar suporte a datas de vencimento para as tarefas.


