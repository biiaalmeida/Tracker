## UC06 - Visualizar Funcionário

### 1. Descrição

É a funcionalidade que permite o Gerente visualizar as informações do funcionário selecionado. Como nome, CPF, email, telefone, função e carga horária. O Gerente pode editar ou remover o funcionário.

### 2. Importância

Média

### 3. Ator Primário / Ator Secundário

- Primário: Gerente

### 4. Pré-condições

- Funcionário cadastrado no sistema;
- Gerente precisa estar autenticado no sistema;

### 4. Pós-condições

- Funcionário visualizado;
- Funcionário editado ou removido.

### 5. Fluxo Principal

#### P6. Visualizar Funcionário
##### P6.1 Gerente seleciona o funcionário;
##### P6.2 Sistema exibe as informações do funcionário;
##### P6.3 Gerente seleciona a opção "Editar Funcionário"; A1
##### P6.4 Gerente seleciona a opção "Remover Funcionário"; A2
##### P6.5 Sistema exibe a mensagem "Funcionário atualizado com sucesso!"; P6.2
##### P6.6 Caso de uso finalizado.

### 6. Fluxo Alternativo

#### A1. Editar Funcionário
##### A1.1 Gerente seleciona "Editar Funcionário"; P6.5

#### A2. Remover Funcionário
##### A2.1 Gerente seleciona "Remover Funcionário"; P6.5

### 7. Fluxo de Exceção

#### Não há fluxos de exceção para este caso de uso.

### 8. Regras de Negócio

#### RN01 - Um gerente pode gerenciar múltiplos funcionários.
#### RN02 - Um funcionário é gerenciado por apenas um gerente.

-------------------------------------
### Histórico

- Data: 30/04/2026 - Versão Inicial - Responsável: Letícia Morais