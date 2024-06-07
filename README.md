# API 5° Semestre - Quarks Team

## Tema

Dashboard Web de Análise de Faturas de Energia, Água e Gás

## Contexto

A TecSUS realiza a coleta e processamento de contas de energia, água e gás para diversas empresas dos setores do atacado e varejo. Cada conta coletada precisa ter todos os seus campos digitados e salvos em banco de dados para eventuais consultas e análises técnicas/financeiras que podem trazer ao cliente oportunidades de redução de custos e alteração de contratos. Cada unidade do cliente pode possuir vários contratos (água, energia ou gás), cada contrato pode possuir uma ou mais contas (faturas de água, energia ou gás) por mês. Todos esses contratos estão ligados a uma concessionária de abastecimento. A TecSUS possui uma base de dados de unidades, contratos, contas e concessionárias desestruturada em arquivo texto, a empresa tem interesse em aplicar técnicas de ETL e utilizar ferramentas de visualização de dados do mercado.

## Desafio

Este projeto consiste no desenvolvimento de um dashboard web de alta complexidade para análise e exibição de dados de faturas de energia, água. O objetivo é fornecer insights valiosos para empresas clientes da TecSUS, permitindo a redução de custos e otimização de contratos.

# Projeto de Gerenciamento de Consumo

## Visão Geral
Este projeto visa desenvolver um sistema para gerenciar o consumo de recursos (água e energia) de unidades, concessionárias e contratos, com a capacidade de gerar relatórios e alertas baseados nos dados coletados. Além disso, será implementada uma esteira de DevOps para assegurar a eficiência e rastreabilidade do desenvolvimento.

## Requisitos

### R1: Extrair, Transformar e Carregar os dados de Unidades, Concessionárias, Contratos e Contas.

### R2: Relatório de consumo total de água mensal, anual e média. (acima da média dos últimos 3 meses).

### R3: Relatório de consumo total de energia mensal, anual e média. (acima da média dos últimos 3 meses).

### R4: Geração de alertas de consumo total de água acima da média (acima da média dos últimos 3 meses).

### R5: Geração de alertas do consumo total de energia do tipo A mensal, anual e média.

### R6: Geração de alertas do consumo total de energia do tipo B mensal, anual e média.

### R7: Geração de alertas do consumo total de esgoto mensal, anual e média.

### R8: Geração de alertas do demanda de energia tipo A mensal.

### R9: Desenvolver e aplicar uma esteira de DevOps de acordo com a solução proposta.


## Tabela de Requisitos e Épicos

| Requisito | Épico que Resolve                          |
|-----------|--------------------------------------------|
| R1        | Épico 1: ETL (Extrair, Transformar e Carregar) de Dados |
| R2        | Épico 2: Dashboards de Consumo, Épico 3: Relatórios de Consumo |
| R3        | Épico 2: Dashboards de Consumo, Épico 3: Relatórios de Consumo |
| R4        | Épico 4: Alertas de Consumo                |
| R5        | Épico 4: Alertas de Consumo                |
| R6        | Épico 4: Alertas de Consumo                |
| R7        | Épico 4: Alertas de Consumo                |
| R8        | Épico 4: Alertas de Consumo                |
| R9        | Épico 5: Esteira de DevOps                 |

## Épicos

### Épico 1: ETL (Extrair, Transformar e Carregar) de Dados
#### Descrição
Este épico cobre o desenvolvimento e implementação de um processo ETL para extrair dados de diferentes fontes, transformá-los conforme necessário e carregá-los em um banco de dados centralizado.

#### Requisitos Resolvidos
- **R1:** Extrair, Transformar e Carregar os dados de Unidades, Concessionárias, Contratos e Contas.

#### Funcionalidades Implementadas
- Definição da estrutura do banco de dados para armazenar dados de Unidades, Concessionárias, Contratos e Contas.
- Desenvolvimento de scripts de extração de dados de diferentes fontes (e.g., arquivos CSV, APIs).
- Implementação da transformação de dados (e.g., limpeza, normalização).
- Desenvolvimento de processos de carga de dados no banco de dados centralizado.
- Automatização do processo ETL utilizando ferramentas como Apache Airflow ou similares.

### Épico 2: Dashboards de Consumo
#### Descrição
Este épico envolve a criação de dashboards detalhando o consumo total de água e energia de forma mensal, anual e média.

#### Requisitos Resolvidos
- **R2:** Relatório de consumo total de água mensal, anual e média. (acima da média dos últimos 3 meses).
- **R3:** Relatório de consumo total de energia mensal, anual e média. (acima da média dos últimos 3 meses).

#### Funcionalidades Implementadas
- Desenvolvimento de dashboards mensais, anuais e cálculo de média de consumo de água.
- Desenvolvimento de dashboards mensais, anuais e cálculo de média de consumo de energia.

### Épico 3: Relatórios de Consumo
#### Descrição
Este épico envolve a criação de relatórios detalhando o consumo total de água e energia de forma mensal, anual e média.

#### Requisitos Resolvidos
- **R2:** Relatório de consumo total de água mensal, anual e média. (acima da média dos últimos 3 meses).
- **R3:** Relatório de consumo total de energia mensal, anual e média. (acima da média dos últimos 3 meses).

#### Funcionalidades Implementadas
- Desenvolvimento de relatórios mensais, anuais e cálculo de média de consumo de água.
- Desenvolvimento de relatórios mensais, anuais e cálculo de média de consumo de energia.

### Épico 4: Alertas de Consumo
#### Descrição
Este épico abrange a implementação de um sistema de geração de alertas para notificar consumo acima da média dos últimos três meses.

#### Requisitos Resolvidos
- **R4:** Geração de alertas de consumo total de água acima da média (acima da média dos últimos 3 meses).
- **R5:** Geração de alertas do consumo total de energia do tipo A (acima da média dos últimos 3 meses).
- **R6:** Geração de alertas do consumo total de energia do tipo B, (acima da média dos últimos 3 meses).
- **R7:** Geração de alertas de consumo total de esgoto acima da média (acima da média dos últimos 3 meses).
- **R8:** Geração de alertas do demanda de energia tipo A mensal.

#### Funcionalidades Implementadas
- Definição dos critérios para identificação de consumo acima da média.
- Desenvolvimento do mecanismo de cálculo da média de consumo dos últimos três meses.
- Implementação do sistema de notificação de alertas (dashboard).
- Testes e validação do sistema de alertas.

### Épico 5: Esteira de DevOps
#### Descrição
Este épico foca no desenvolvimento e aplicação de uma esteira de DevOps para garantir a eficiência, rastreabilidade e qualidade do desenvolvimento.

#### Requisitos Resolvidos
- **R9:** Desenvolver e aplicar uma esteira de DevOps de acordo com a solução proposta.

#### Funcionalidades Implementadas
- Configuração do controle de versão com Git (Estratégia de Branches).
- Rastreabilidade dos requisitos através das tasks.
- Implementação de integração contínua (CI) utilizando ferramentas como GitHub Actions.
- Documentação do processo de DevOps e treinamento da equipe.
  
<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Solução

Nós da equipe Quarks vamos desenvolver um sistema web que irá permitir que o cliente faça o o input dos aquivos brutos com os dados de sua conta e visualize todos os dashbords e relatórios.

<p align="right">(<a href="#top">Scroll to top</a>)</p>

<hr/>

### Sprint Menu
<ul>
  <li><a href="https://github.com/quarks-team/Projeto-Integrador-TecSUS?tab=readme-ov-file#sprint-1">SPRINT 1</a></li>
  <li><a href="https://github.com/quarks-team/Projeto-Integrador-TecSUS?tab=readme-ov-file#sprint-2">SPRINT 2</a></li>
  <li><a href="https://github.com/quarks-team/Projeto-Integrador-TecSUS?tab=readme-ov-file#sprint-3">SPRINT 3</a></li>
  <li><a href="https://github.com/quarks-team/Projeto-Integrador-TecSUS?tab=readme-ov-file#sprint-4">SPRINT 4</a></li>
</ul>

## Schedule

| Event             | Date           |
| ----------------- | -------------- |
| Kick-off          | 04/03 to 08/03 |
| Sprint 1          | 25/03 to 15/04 |
| Sprint 2          | 15/04 to 06/05 |
| Sprint 3          | 06/05 to 26/05 |
| Sprint 4          | 27/05 to 17/06 |
| Feira de Soluções | 27/06          |

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Product Backlog

<table>
  <thead>
    <tr>
      <th>Rank</th>
      <th>Requisito</th>
      <th>Prioridade</th>
      <th>User Story</th>
      <th>Story Point</th>
      <th>Sprint</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Infraestrutura de dados e ETL</td>
      <td>Alta</td>
      <td>Como usuário da plataforma, quero carregar as informações das contas de água e energia de arquivos csv para o banco de dados, para que possamos analisar e visualizar os dados de consumo de água.</td>
      <td>8</td>
      <td>1</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Relatório de consumo (Energia)</td>
      <td>Alta</td>
      <td>Como usuário da plataforma, quero visualizar gráficos e tabelas que representem o consumo mensal e anual de energia, para que eu possa compreender as tendências e identificar oportunidades de economia.</td>
      <td>5</td>
      <td>1</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Relatório de consumo (Água)</td>
      <td>Alta</td>
      <td>Como usuário da plataforma, quero visualizar gráficos e tabelas que representem o consumo mensal e anual de água, para que eu possa compreender as tendências e identificar oportunidades de economia.</td>
      <td>5</td>
      <td>2</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Infraestrutura de dados e ETL</td>
      <td>Alta</td>
      <td>Como usuário da plataforma, quero subir os arquivos csv em um sistema, para que possa analisar as métricas concernentes as faturas de água e energia em gráficos e relatorios.</td>
      <td>8</td>
      <td>2</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Alertas de Consumo</td>
      <td>Alta</td>
      <td>Como usuário da plataforma, quero receber alertas acerca dos consumo, para tomar medidas de redução de custos e alteração de contratos.</td>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <td>6</td>
      <td>Plataforma Web</td>
      <td>Média</td>
      <td>Como usuário da plataforma, quero subir arquivos e visualizar relatórios em uma unica ferramenta, para que possa fazer análises estratégicas em tempo real.</td>
      <td>6</td>
      <td>2</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Alertas de Consumo</td>
      <td>Média</td>
      <td>Como usuário da plataforma, quero receber alertas de alto consumo por email, para que possa tomar medidas de redução de custos.</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <td>8</td>
      <td>Infraestrutura de dados e ETL</td>
      <td>Baixa</td>
      <td>Como usuário da plataforma, quero baixar os relatórios, para que possa fazer a análises das informações das faturas.</td>
      <td>5</td>
      <td>4</td>
    </tr>
  </tbody>
</table>

## Task Board
Para garantir o gerenciamento centralizado de todas as atividades do projeto, estamos utilizando o Jira Software como nossa ferramenta principal de monitoramento de tarefas e acompanhamento de projetos.

[Link para o Projeto no Jira](https://gabriel-timoteo-dos-santos.atlassian.net/jira/software/projects/API5/boards/3)

# Epics
O projeto será estruturado em 4 épicos, nos quais serão atribuídas as respectivas tarefas relacionadas a cada um desses temas. Essa divisão facilitará a organização e execução de todas as etapas do projeto.

| Épico                              | Tema                                                                                                                                          |
|------------------------------------| ----------------------------------------------------------------------------------------------------------------------------------------------|
| Infraestrutura de Dados e ETL      | Criação da base de dados e desenvolvimento do processo de ETL para garantir que os dados sejam coletados, tratados e carregados corretamente. |
| Desenvolvimento de Dashboards      | Desenvolvimento de dashboards interativos para visualização e análise de dados de contas de água, energia e gás.                              |
| Plataforma Web e Relatórios        | Criação de uma plataforma web para hospedar os dashboards e relatórios, fornecendo uma interface para análise de dados.                       |
| Sistema de Alertas e Documentações | Implementação de um sistema de alertas para consumo anormal e conclusão do projeto com documentação e testes finais.                          |

<p align="right">(<a href="#top">Scroll to top</a>)</p>

---

## Especificações Técnicas do projeto
[Loading]

---
<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Time

| Avatar                                                     | Student               | Function         | GitHub                                                                 | LinkedIn                                                                          |
| ---------------------------------------------------------- | --------------------- | ---------------- | ---------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| <img src = "./Documents/Team/gabriel.png" width="60" >    | **Gabriel Timoteo**   | _Product Owner_  | [![](https://bit.ly/3f9Xo0P)](https://github.com/Michaelfss/gatimoteo) | [![](https://bit.ly/2P1ZogM)](https://www.linkedin.com/in/gabriel-timoteo-santos) |
| <img src = "./Documents/Team/felipe.png" width="60" >     | **Felipe Augusto**    | _Scrum Master_   | [![](https://bit.ly/3f9Xo0P)](https://github.com/FelipeASousa)         | [![](https://bit.ly/2P1ZogM)]()                                                   |
| <img src = "./Documents/Team/lucas.png" width="60" >      | **Lucas Barcelos**    | _Developer Team_ | [![](https://bit.ly/3f9Xo0P)](https://github.com/lucassbarcelos)       | [![](https://bit.ly/2P1ZogM)]()                                                   |
| <img src = "./Documents/Team/leonardo.png" width="60" >   | **Leonardo Adler**    | _Developer Team_ | [![](https://bit.ly/3f9Xo0P)](https://github.com/LeoAdlerr)            | [![](https://bit.ly/2P1ZogM)](https://www.linkedin.com/in/leonardo-adler-silva-6b4a37228/)                                                   |
| <img src = "./Documents/Team/daniela.jpg" width="60" >    | **Daniela Meirelles** | _Developer Team_ | [![](https://bit.ly/3f9Xo0P)](https://github.com/DanielaMeirelles)     | [![](https://bit.ly/2P1ZogM)](https://www.linkedin.com/in/daniela-meirelles-1990/)                                                   |
| <img src = "./Documents/Team/guilherme.jpeg" width="60" > | **Guilherme Alves**   | _Developer Team_ | [![](https://bit.ly/3f9Xo0P)](https://github.com/guilherme0066)        | [![](https://bit.ly/2P1ZogM)]()                                                   |
| <img src = "./Documents/Team/felipe_sobral.jpeg" width="60" > | **Felipe Sobral**     | _Developer Team_ | [![](https://bit.ly/3f9Xo0P)](https://github.com/SoSoJigsaw)           | [![](https://bit.ly/2P1ZogM)]()                                                   |
<p align="right">(<a href="#top">Scroll to top</a>)</p>

---
## Repositórios
- [Frontend](https://github.com/quarks-team/projeto_integrador_tecsus_frontend/tree/main)
- [Backend](https://github.com/quarks-team/projeto-integrador-tecsus-backend)
- [Database](https://github.com/quarks-team/Projeto-Integrador-TecSUS-Database)

---
## Tecnologias utilizadas
<details>
  <summary>Ferramenta de Gestão de Projetos</summary>
  
- [Jira](https://www.atlassian.com/br/software/jira)
</details>
<details>
<summary>Front-End</summary>
  
- [Power Bi](https://powerbi.microsoft.com/pt-br/desktop/)
- [Vue](https://vuejs.org/)
- [Typescript](https://www.typescriptlang.org/)
- [HTML](https://www.w3schools.com/css/)
- [CSS](https://www.w3schools.com/css/)

</details>

<details>
<summary>Back-End</summary>

- [Typescript](https://www.typescriptlang.org/)

- [Node](https://nodejs.org/en)

</details>

<details>
<summary>Database</summary>

- [MySQL](https://www.mysql.com/))
</details>

<details>
<summary>Meetings and Communication</summary>

- [Discord](https://discord.com/?msclkid=b4f5af84b8f811ecbd81c127a0ae68a7)

- [Whatsapp](https://www.whatsapp.com/)

- [Slack](https://slack.com/intl/pt-br/?msclkid=c00e628eb8f811ecaef374bb86d7f056)
</details>

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Sprint 1
### 25/03 to 15/04
### Épicos
<ul>
  <li>Infraestrutura de Dados e ETL</li>
  <li>Desenvolvimento de Dashboards</li>
</ul>

### Tecnologias Utilizadas
- [Typescript](https://www.typescriptlang.org/)
- [Power Bi](https://powerbi.microsoft.com/pt-br/desktop/)
- [Node](https://nodejs.org/en)
- [MySQL](https://www.mysql.com/)
  
| Sprint   | Objetivo                                                                                          | Entrega                                                                                                                                                                          |
| -------- | --------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sprint 1 | Desenvolver a estrutura base do projeto e criar um modelo de dashboard para visualização dos dados. | **Modelagem e Desenvolvimento do Banco de Dados:**<br>• Criação do esquema do banco de dados para suportar unidades, concessionárias, contratos e contas.<br>• Implementação de tabelas e relações entre elas.<br><br>**Desenvolvimento do ETL:**<br>• Implementação de scripts em Python para a extração dos dados dos arquivos de texto.<br>• Desenvolvimento da lógica de transformação para padronizar e limpar os dados.<br>• Carregamento dos dados transformados no banco de dados.<br><br>**Dashboard de Energia:**<br>• Desenvolvimento do dashboard para a conta de energia elétrica.<br>• Implementação de visualizações de dados (gráficos, tabelas) para consumo mensal e anual.<br><br>**Testes Iniciais:**<br>• Realização de testes iniciais para validar a funcionalidade do ETL e do banco de dados.<br>• Verificação da precisão dos dados no dashboard da conta de água.<br><br>**Documentação Inicial:**<br>• Criação da documentação básica do projeto, incluindo a arquitetura do sistema e descrição dos processos de ETL.|

---
## Burndown
<img src="https://github.com/quarks-team/Projeto-Integrador-TecSUS/blob/main/Documents/Burndown/BURNDOWN_SPRINT1.png?raw=true"/>

---
## MER Database
[Modelagem do Banco](https://github.com/quarks-team/Projeto-Integrador-TecSUS-Database/blob/main/modelagem_banco_API_v.05.png)

---
## Dashboard Screen
<img src="https://github.com/quarks-team/Projeto-Integrador-TecSUS/blob/main/Documents/Mockup/DASHBOARD_1.png?raw=true"/>
<img src="https://github.com/quarks-team/Projeto-Integrador-TecSUS/blob/main/Documents/Mockup/DASHBOARD_2.png?raw=true"/>

---

## Sprint 2
### 15/04 to 05/05
### Épicos
<ul>
  <li>Infraestrutura de Dados e ETL</li>
  <li>Desenvolvimento de Dashboards</li>
  <li>Plataforma Web e Relatórios</li>
</ul>

### Tecnologias Utilizadas
- [Typescript](https://www.typescriptlang.org/)
- [Power Bi](https://powerbi.microsoft.com/pt-br/desktop/)
- [Node](https://nodejs.org/en)
- [MySQL](https://www.mysql.com/)
- [Vue](https://vuejs.org/)
  
| Sprint   | Objetivo                                                                                          | Entrega                                                                                                                                                                          |
| -------- | --------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sprint 2 | Estabelecer a base da plataforma web e desenvolver o dashboard de uma das contas restantes.       | **Desenvolvimento da plataforma web (Parte 1):**<br>• Configuração inicial da plataforma web (framework, autenticação de usuários, layout básico).<br>• Desenvolvimento da estrutura básica de navegação (menus, páginas básicas).<br><br>**Dashboard da Conta de Água:**<br>• Desenvolvimento de um dashboard inicial para a visualização dos dados da conta de água.<br>• Implementação de gráficos e tabelas para exibir consumo e custos mensais e anuais.<br><br>**Testes no ETL (Parte 1):**<br>• Implementação de testes unitários para as funcionalidades já desenvolvidas do ETL.<br>• Documentação inicial dos testes e resultados.<br><br>**Documentação (Parte 1):**<br>• Início da documentação técnica do sistema, com foco na arquitetura e nas decisões de design. |

---
## Burndown
<img src="https://github.com/quarks-team/Projeto-Integrador-TecSUS/blob/main/Documents/Burndown/BURNDOWN_SPRINT2.png?raw=true"/>

---
## Atualização MER Database
<img src="https://github.com/quarks-team/Projeto-Integrador-TecSUS/blob/main/Documents/MER/modelagem_banco_API_v.05.png?raw=true"/>

---
## Mockup Plataforma
[Figma](https://www.figma.com/file/8rOktvbSKRRPjosUsZI19f/Tecsus?type=design&node-id=0%3A1&mode=design&t=QOGkxSUSIHqO3zUM-1)

---
## Dashboard de Água
[Água](https://app.powerbi.com/links/xkuLmZTQKZ?ctid=cf72e2bd-7a2b-4783-bdeb-39d57b07f76f&pbi_source=linkShare)

---
## Plataforma

<img src="https://github.com/quarks-team/Projeto-Integrador-TecSUS/blob/main/Documents/Gifs/gif-dash-agua.gif?raw=true"/>
<img src="https://github.com/quarks-team/Projeto-Integrador-TecSUS/blob/main/Documents/Gifs/gif-dash-luz.gif?raw=true"/>



## Sprint 3
### 06/05 to 26/05
### Épicos
<ul>
  <li>Infraestrutura de Dados e ETL</li>
  <li>Desenvolvimento de Dashboards</li>
  <li>Plataforma Web e Relatórios</li>
  <li>Sistema de Alertas</li>
</ul>

### Tecnologias Utilizadas
- [Typescript](https://www.typescriptlang.org/)
- [Power Bi](https://powerbi.microsoft.com/pt-br/desktop/)
- [Node](https://nodejs.org/en)
- [MySQL](https://www.mysql.com/)

| Sprint   | Objetivo                                                                                          | Entrega                                                                                                                                                                          |
| -------- | --------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sprint 3 | Completar os dashboards e iniciar o desenvolvimento do sistema de alertas.                        | **Desenvolvimento da plataforma web (Parte 2):**<br>• Aprimoramento do layout e da experiência do usuário na plataforma web.<br>• Implementação de funcionalidades adicionais de interação com os relatórios e dashboards.<br>• Implementação de visualizações de dados (gráficos, tabelas) para consumo mensal e anual.<br><br>**Relatório de Consumo:**<br>• Desenvolvimento de relatórios de consumo que integram dados de água, energia e gás.<br>• Possibilidade de visualizar relatórios mensais, anuais e médias de consumo.<br><br>**Início do Sistema de Alertas:**<br>• Desenvolvimento da lógica para identificar consumos acima da média.<br>**Testes no ETL (Parte 2):**<br>• Continuação da implementação de testes unitários para novas funcionalidades do ETL.<br>• Atualização da documentação de testes. |

---
## Burndown
<img src="https://github.com/quarks-team/Projeto-Integrador-TecSUS/blob/main/Documents/Burndown/BURNDOWN_SPRINT3.png?raw=true"/>

---
## Contribuições dos membros

### Tarefas Concluídas

<p>Pontos Concluídos/ Pontos totais</p>
<ul>
  <li>Daniela Meirelles - 8/8</li>
  <li>Felipe Augusto (Master) - 13/13</li>
  <li>Felipe Sobral - 9/9</li>
  <li>Gabriel Timóteo (Product Owner) - 0/5</li>
  <li>Gulherme A. Cursino - 6/6</li>
  <li>Leonardo Adler - 23/23</li>
  <li>Lucas Barcelos - 11/11</li>
</ul>

### Tarefas por membro
![image](https://github.com/quarks-team/Projeto-Integrador-TecSUS/assets/79467858/4aac8d8b-2e20-4fde-a98e-bfc3dce5320c)

### Commits por Repositório

#### Banco de Dados
![image](https://github.com/quarks-team/Projeto-Integrador-TecSUS/assets/79467858/11628620-55a6-4a2c-b20e-0bb76f8a42fe)

#### Frontend
![image](https://github.com/quarks-team/Projeto-Integrador-TecSUS/assets/79467858/cfd4c5a6-767c-4eab-a37a-a4a77c8ba874)


#### Backend
![image](https://github.com/quarks-team/Projeto-Integrador-TecSUS/assets/79467858/221d2e9b-629b-413c-82f9-a64358971dd1)


#### Repositório de Documentação
![image](https://github.com/quarks-team/Projeto-Integrador-TecSUS/assets/79467858/e546c498-bf58-407b-a752-5aa0a4f962c5)

## Sprint 4
### 15/04 to 05/05
### Épicos
<ul>
  <li>Infraestrutura de Dados e ETL</li>
  <li>Desenvolvimento de Dashboards</li>
  <li>Plataforma Web e Relatórios</li>
  <li>Sistema de Alertas</li>
</ul>

### Tecnologias Utilizadas
- [Typescript](https://www.typescriptlang.org/)
- [Power Bi](https://powerbi.microsoft.com/pt-br/desktop/)
- [Node](https://nodejs.org/en)
- [MySQL](https://www.mysql.com/)

| Sprint   | Objetivo                                                                                          | Entrega                                                                                                                                                                          |
| -------- | --------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sprint 4 | Finalizar o sistema de alertas, completar a documentação e realizar testes finais.                | **Completo Sistema de Alertas:**<br>• Finalização do sistema de alertas, incluindo a interface de usuário para configuração dos alertas.<br>• Testes e ajustes no sistema de notificação.<br><br>**Aprimoramento da Plataforma Web:**<br>• Testes de usabilidade e ajustes finais na plataforma web.<br>• Implementação de feedbacks dos usuários obtidos nas sprints anteriores.<br><br>**Documentação Completa do Produto:**<br>• Finalização da documentação técnica, incluindo detalhes de implementação e uso.<br>• Criação de documentação para usuários finais (manuais, FAQs).<br><br>**Testes Finais no ETL e na Plataforma:**<br>• Testes de integração para garantir que o ETL está funcionando corretamente com a plataforma web.<br>• Testes de carga e performance para validar a estabilidade e escalabilidade do sistema.<br><br>**Revisão e Correções Finais:**<br>• Revisão de todo o código e funcionalidades desenvolvidas.<br>• Correção de bugs e problemas encontrados nos testes.<br><br>**Preparação para o Lançamento:**<br>• Preparação do ambiente de produção.<br>• Planejamento do lançamento e comunicação com os clientes. |

---
## Burndown
<img src=""/>

---

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Licença
Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
