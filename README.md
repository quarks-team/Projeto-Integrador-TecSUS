# API 5° Semestre - Quarks Team

## Tema

Dashboard Web de Análise de Faturas de Energia, Água e Gás

## Contexto

A TecSUS realiza a coleta e processamento de contas de energia, água e gás para diversas empresas dos setores do atacado e varejo. Cada conta coletada precisa ter todos os seus campos digitados e salvos em banco de dados para eventuais consultas e análises técnicas/financeiras que podem trazer ao cliente oportunidades de redução de custos e alteração de contratos. Cada unidade do cliente pode possuir vários contratos (água, energia ou gás), cada contrato pode possuir uma ou mais contas (faturas de água, energia ou gás) por mês. Todos esses contratos estão ligados a uma concessionária de abastecimento. A TecSUS possui uma base de dados de unidades, contratos, contas e concessionárias desestruturada em arquivo texto, a empresa tem interesse em aplicar técnicas de ETL e utilizar ferramentas de visualização de dados do mercado.

## Desafio

Este projeto consiste no desenvolvimento de um dashboard web de alta complexidade para análise e exibição de dados de faturas de energia, água. O objetivo é fornecer insights valiosos para empresas clientes da TecSUS, permitindo a redução de custos e otimização de contratos.

## Requisitos

<table>
  <thead>
    <tr>
      <th>Requisitos Funcionais</th>
      <th>Requisitos Não Funcionais</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <ul>
          <li><strong>ETL(Extract, Trasnform, Load):</strong> Implementação de um sistema robusto para extração, transformação e carregamento dos dados das Faturas e dos dados de Unidades, Concessionárias e Contratos.</li>
          <li><strong>Relatório de consumo:</strong> Capacidade de gerar relatórios detalhados do consumo total e médio de água e energia.</li>
          <li><strong>Alertas de Consumo:</strong> Desenvolvimento de um sistema de alertas para consumo acima da média dos últimos três meses.</li>
        </ul>  
      </td>
      <td>
        <ul>
          <li><strong>Esteira de DevOps:</strong> Utilização de práticas de DevOps para assegurar a integração e entrega contínua do projeto.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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

| Rank | Prioridade | User Story | Tasks | Story Points | Sprint |
|------|------------|------------|-------|--------------|--------|
| 1    | Alta       | Como administrador, eu quero receber alertas personalizados para diferentes tipos de consumo (energia, água, esgoto) para monitorar e agir rapidamente sobre desvios de consumo. | . Adicionar Alertas de esgoto <br> . Criar relatório de alertas de demanda <br> . Adicionar alerta de demandas no endpoint de alertas <br> . Criar Trigger para popular tabela de alertas de demanda <br> . Criar uma tabela para alertas de demanda <br> . Esgoto: Criar trigger para alerta de consumo acima média dos últimos 3 meses <br> . Água: Criar trigger para alerta de consumo acima média dos últimos 3 meses <br> . Energia: Criar trigger para alerta de consumo acima média dos últimos 3 meses <br> . Criar componente do alerta <br> . Criar endpoint para buscar alertas <br> . Adicionar ícone de notificação de alertas | 13 | 0 |
| 2    | Alta       | Como usuário, eu quero que o sistema evite duplicidade de dados para garantir a integridade das informações carregadas. | . Inserir state da requisição de upload <br> . Criar funcionalidade de impedimento de carga duplicada no banco de dados <br> . Fazer verificação de duplicidade de datas na tabela de tempo <br> . Testar requisição para API Node | 8 | 0 |
| 3    | Alta       | Como administrador, eu quero visualizar dashboards de consumo de energia e água para analisar e comparar o consumo entre diferentes unidades e períodos. | . Inserir dashboard PowerBI de luz na interface usando <iframe> <br> . Inserir dashboard PowerBI de água na interface usando <iframe> <br> . Melhorar o Dashboard de Energia <br> . Definição dos gráficos (mockup) do Dashboard (Água) <br> . Desenvolvimento do Dashboard (Água) <br> . Criar componenete para o dashboard de luz <br> . Criar componente para o dashboard de água | 21 | 0 |
| 4    | Média      | Como usuário, eu quero que a plataforma seja responsiva e funcione bem em diferentes dispositivos para facilitar o acesso e o uso do sistema. | . Ajustar responsividade dos elementos das páginas do frontend | 5 | 0 |
| 5    | Alta       | Como desenvolvedor, eu quero garantir que o código seja de alta qualidade e facilmente rastreável para facilitar a manutenção e futuras implementações. | . Implementar análises estáticas no frontend <br> . Atingir alguma cobertura de código do backend <br> . Atingir meta de 25% de cobertura de código do frontend <br> . Teste BigBang <br> . Teste TopDown <br> . Teste BottomUp <br> . Refatorar CI frontEnd <br> . Finalizar documentação do ETL <br> . Documentação para rastreabilidade | 13 | 0 |
| 6    | Alta       | Como administrador, eu quero realizar cargas e extrações de dados de forma eficiente para garantir que todas as informações estejam atualizadas e disponíveis para análise. | . Criar funcionalidade de carga na tabela de água <br> . Criar funcionalidade de carga na tabela de energia <br> . Carregamento dos dados do contrato de energia <br> . Carregamento dos dados do contrato de água <br> . Carregamento dos dados da conta de energia <br> . Transformação dos dados do contrato de energia <br> . Transformação dos dados do contrato de água <br> . Transformação dos dados da conta de energia <br> . Extração do contrato de energia <br> . Extração da conta de energia <br> . Extração do contrado de água | 21 | 0 |
| 7    | Média      | Como administrador, eu quero que o sistema me permita exportar dados em diferentes formatos para facilitar a análise externa e a criação de relatórios. | . Criar exportação de relatório no power bi <br> . Criar um botão de exportar arquivo (pdf, xlsx, csv) | 8 | 0 |
| 8    | Média      | Como usuário, eu quero acessar logs detalhados sobre o processamento do ETL para entender e solucionar possíveis problemas de carga de dados. | . Gerar logs para usuário a respeito do processamento do ETL <br> . Testes de integração para garantir que o ETL está funcionando corretamente com a plataforma web (testar endpoints) <br> . Criar documentação da regra de negócio do ETL | 13 | 0 |
| 9    | Alta       | Como desenvolvedor, eu quero automatizar o processo de deploy e integração contínua para garantir uma entrega contínua e confiável do sistema. | . Devops <br> . Deploy Backend <br> . Deploy FrontEnd <br> . Criação da pipeline de CI para rodar testes | 8 | 0 |
| 10   | Baixa      | Como usuário, eu quero que a plataforma tenha uma navegação intuitiva para facilitar o acesso às diferentes funcionalidades. | . Desenvolvimento da Estrutura Básica de Navegação <br> . Configuração Inicial da Plataforma Web <br> . Desenho da(s) tela(s) da plataforma Web | 5 | 0 |



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
