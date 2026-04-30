## UC01 - Visualizar Card

### 1. Descrição

É a funcionalidade que permite o funcionário visualizar a informações do tarefa selecionada. Como título, descrição, data de criação, data de conclusão, tags, status e o responsável pela tarefa. O funcionário pode iniciar, concluir ou pausar a tarefa.

### 2. Importância

Alta

### 3. Ator Primário / Ator Secundário

- Primário: Funcionário

### 4. Pré-condições

- Card cadastrado no sistema;
- Funcionário precisa estar autenticado no sistema;

### 4. Pós-condições

- Tarefa visualizada;
- Tarefa iniciada, pausada ou concluída.

### 5. Fluxo Principal

#### P1. Visualizar Card
#### P1.1 Funcionário seleciona o card da tarefa;
#### P1.2 Sistema exibe as informações do card;
#### P1.3 Funcionário seleciona a opção "Iniciar Tarefa"; A1
#### P1.4 Funcionário seleciona a opção "Pausar Tarefa"; A2
#### P1.5 Funcionário seleciona a opção "Concluir Tarefa"; A3
#### P1.7 Sistema exibe a mensagem "Tarefa atualizada com sucesso!";
#### P1.8 Caso de uso finalizado.

### 6. Fluxo Alternativo

#### A1. Iniciar Tarefa
##### A1.1 Atendente seleciona "Iniciar Tarefa"; P1.7

#### A2. Pausar Tarefa
##### A2.1 Atendente seleciona "Pausar Tarefa"; P1.

#### A3. Concluir Tarefa
##### A3.1 Atendente seleciona "Concluir Tarefa"; P1.7

### 7. Fluxo de Exceção

#### Não há fluxos de exceção para este caso de uso.

### 8. Regras de Negócio

#### RN02 - Um funcionário pode possuir múltiplos cards.
#### RN03 - Um card é possuído por apenas um funcionário.

-------------------------------------
### Histórico

- Data: 30/04/2026 - Versão Inicial - Responsável: Letícia Morais
