## UC03 - Gerar Relatório

### 1. Descrição

É o processo em que o Gerente gera relatórios no Sistema Tracker para acompanhar o desempenho dos funcionários, cards concluídos, cards pausados, cards iniciados e demais atividades registradas no sistema.

### 2. Importância

Média

### 3. Ator Primário / Ator Secundário

- Primário: Gerente

### 4. Pré-condições

- Gerente precisa estar autenticado no sistema;
- Devem existir funcionários cadastrados no sistema;
- Devem existir cards registrados no sistema;
- Os cards devem possuir status associado.

### 4. Pós-condições

- Relatório gerado com sucesso ou operação cancelada;
- Dados de desempenho exibidos ao Gerente;
- Relatório registrado com título, data de geração e Gerente responsável.

### 5. Fluxo Principal

#### P1. Gerar Relatório

##### P1.1 Gerente seleciona a opção "Gerar Relatórios";
##### P1.2 Sistema exibe as opções de relatório disponíveis;
##### P1.3 Gerente seleciona o tipo de relatório desejado;
##### P1.4 Sistema solicita os critérios de geração do relatório; A1
##### P1.5 Gerente informa os critérios necessários;
##### P1.6 Sistema busca os dados de funcionários, cards e tags; E1
##### P1.7 Sistema calcula o desempenho com base nos dados encontrados;
##### P1.8 Sistema gera o relatório;
##### P1.9 Sistema exibe o relatório ao Gerente; A2
##### P1.10 Caso de uso finalizado.

### 6. Fluxo Alternativo

#### A1. Filtrar Relatório

##### A1.1 Gerente seleciona a opção "Filtrar Relatórios";
##### A1.2 Sistema exibe opções de filtro por funcionário, período ou tag;
##### A1.3 Gerente escolhe os filtros desejados;
##### A1.4 Sistema aplica os filtros selecionados; P1.6

#### A2. Gerar Novo Relatório

##### A2.1 Gerente seleciona a opção "Gerar Novo Relatório";
##### A2.2 Sistema retorna para a tela de seleção de relatório; P1.2

#### A3. Cancelar Geração

##### A3.1 Gerente seleciona a opção "Cancelar";
##### A3.2 Sistema cancela a operação;
##### A3.3 Caso de uso finalizado.

### 7. Fluxo de Exceção

#### E1. Dados não encontrados

##### E1.1 Sistema exibe a mensagem "Não há dados suficientes para gerar o relatório.";
##### E1.2 Sistema retorna para a tela de opções de relatório; P1.2

#### E2. Filtro inválido

##### E2.1 Sistema exibe a mensagem "Filtro inválido ou período incorreto.";
##### E2.2 Sistema solicita novamente os critérios de filtro; P1.4

#### E3. Erro ao gerar relatório

##### E3.1 Sistema exibe a mensagem "Erro ao gerar relatório. Tente novamente.";
##### E3.2 Sistema retorna para a tela de geração de relatórios; P1.2

### 8. Regras de Negócio

#### RN01 - Apenas Gerentes podem gerar relatórios;
#### RN02 - O Gerente deve estar autenticado para acessar a funcionalidade;
#### RN03 - O relatório deve utilizar dados de funcionários, cards e tags cadastrados no sistema;
#### RN04 - O relatório pode ser filtrado por funcionário, período ou tag;
#### RN05 - O sistema deve calcular o desempenho com base nos cards iniciados, pausados, finalizados e pendentes;
#### RN06 - Relatórios não devem ser gerados caso não existam dados suficientes;
#### RN07 - Todo relatório gerado deve possuir título, data de geração e Gerente responsável;
#### RN08 - O relatório deve estar associado ao Gerente que realizou sua geração.

-------------------------------------

### Histórico

- Data: 30/04/2026 - Versão Inicial - Responsável: Rubens Alexandre