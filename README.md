# API 5° Semestre - Quarks Team

## Tema

Dashboard Web de Análise de Faturas de Energia, Água e Gás

## Contexto

A TecSUS realiza a coleta e processamento de contas de energia, água e gás para diversas empresas dos setores do atacado e varejo. Cada conta coletada precisa ter todos os seus campos digitados e salvos em banco de dados para eventuais consultas e análises técnicas/financeiras que podem trazer ao cliente oportunidades de redução de custos e alteração de contratos. Cada unidade do cliente pode possuir vários contratos (água, energia ou gás), cada contrato pode possuir uma ou mais contas (faturas de água, energia ou gás) por mês. Todos esses contratos estão ligados a uma concessionária de abastecimento. A TecSUS possui uma base de dados de unidades, contratos, contas e concessionárias desestruturada em arquivo texto, a empresa tem interesse em aplicar técnicas de ETL e utilizar ferramentas de visualização de dados do mercado.

## Desafio

Este projeto consiste no desenvolvimento de um dashboard web de alta complexidade para análise e exibição de dados de faturas de energia, água e gás. O objetivo é fornecer insights valiosos para empresas clientes da TecSUS, permitindo a redução de custos e otimização de contratos.

<p align="right">(<a href="#top">Scroll to top</a>)</p>

<li>Requisitos Funcionais</li>
<ul>
      <li>Extrair, Transformar e Carregar (ETL): Sistema para extrair, transformar e carregar dados de unidades, concessionárias, contratos e contas;</li>
      <li>Relatórios de Consumo: Geração de relatórios de consumo total de água, energia e gás mensal, anual e média;</li>
      <li>Alertas de Consumo: Sistema de alertas para identificar consumos acima da média dos últimos 3 meses;</li>
</ul>

<li>Requisitos Não Funcionais</li>
<ul>
      <li>Esteira de DevOps: Implementação de uma esteira de DevOps para garantir integração contínua e entrega contínua do projeto;</li>
</ul>

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Solução

Nós da equipe Quarks vamos desenvolver um sistema web que irá permitir que o cliente faça o o input dos aquivos brutos com os dados de sua conta e visualize todos os dashbords e relatórios.

Visando solucionar o projeto, o sistema será entregue em quatro sprints:

| Sprint   | Objetivo                      | Entrega                                                                                                                                                                      |
| -------- | ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sprint 1 | Desenvolver a estrutura base do projeto e criar um modelo de dashboad para visualização dos dados | Modelagem e desenvolvimento do banco de dados; Desenvolvimento do ETL que irá coletar, tratar e carregar os dados para nossa base; Dashboard para uma das contas;|
| Sprint 2 | Relatórios de Consumo     | Desenvolver funcionalidades para gerar relatórios de consumo total de água, energia e gás mensal, anual e média para cada cliente.                                               |
| Sprint 3 | Alertas de Consumo        | Desenvolver um sistema de geração de alertas para identificar consumos acima da média dos últimos 3 meses e notificar os usuários.                                               |
| Sprint 4 | DevOps                    | Implementar uma esteira de DevOps para garantir a integração contínua, entrega contínua e automação de testes, visando a eficiência e qualidade do processo de desenvolvimento.  |

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Schedule

| Event             | Date           |
| ----------------- | -------------- |
| Kick-off          | -              |
| Sprint 1          | 25/03 to 15/04 |
| Sprint 2          | 15/04 to 06/05 |
| Sprint 3          | 06/05 to 27/05 |
| Sprint 4          | 27/05 to 17/06 |
| Feira de Soluções | -              |

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Product Backlog

Para garantir o gerenciamento centralizado de todas as atividades do projeto, estamos utilizando o Jira Software como nossa ferramenta principal de monitoramento de tarefas e acompanhamento de projetos.

[Link para o Projeto no Jira](https://gabriel-timoteo-dos-santos.atlassian.net/jira/software/projects/API5/boards/3)

O projeto será estruturado em 4 épicos, nos quais serão atribuídas as respectivas tarefas relacionadas a cada um desses temas. Essa divisão facilitará a organização e execução de todas as etapas do projeto.

| Épico | Tema                      | Sprint   |
| ----- | ------------------------- | -------- |
| 1     | ETL e Integração de Dados | Sprint 1 |
| 2     | Relatórios de Consumo     | Sprint 2 |
| 3     | Alertas de Consumo        | Sprint 3 |
| 4     | DevOps                    | Sprint 4 |

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Especificações Técnicas do projeto

---

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Time

| Avatar                                                        | Student               | Function         | GitHub                                                                 | LinkedIn                                                                          |
| ------------------------------------------------------------- | --------------------- | ---------------- | ---------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| <img src = "./Documentacao/Team/imgMichael.jpg" width="60" >  | **Gabriel Timoteo**   | _Product Owner_  | [![](https://bit.ly/3f9Xo0P)](https://github.com/Michaelfss/gatimoteo) | [![](https://bit.ly/2P1ZogM)](https://www.linkedin.com/in/gabriel-timoteo-santos) |
| <img src = "./Documentacao/Team/imgTiago.jpg" width="60" >    | **Felipe Augusto**    | _Scrum Master_   | [![](https://bit.ly/3f9Xo0P)](https://github.com/FelipeASousa)         | [![](https://bit.ly/2P1ZogM)]()                                                   |
| <img src = "./Documentacao/Team/imgAldrik.jpg" width="60" >   | **Lucas Barcelos**    | _Developer Team_ | [![](https://bit.ly/3f9Xo0P)](https://github.com/lucassbarcelos)       | [![](https://bit.ly/2P1ZogM)]()                                                   |
| <img src = "./Documentacao/Team/imgAna.jpg" width="60" >      | **Leonardo Adler**    | _Developer Team_ | [![](https://bit.ly/3f9Xo0P)](https://github.com/LeoAdlerr)            | [![](https://bit.ly/2P1ZogM)]()                                                   |
| <img src = "./Documentacao/Team/imgEmanuele.jpg" width="60" > | **Daniela Meirelles** | _Developer Team_ | [![](https://bit.ly/3f9Xo0P)](https://github.com/DanielaMeirelles)     | [![](https://bit.ly/2P1ZogM)]()                                                   |
| <img src = "./Documentacao/Team/imgLuiz.jpg" width="60" >     | **Guilherme Alves**   | _Developer Team_ | [![](https://bit.ly/3f9Xo0P)](https://github.com/)                     | [![](https://bit.ly/2P1ZogM)]()                                                   |

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Tecnologias utilizadas

<details>
<summary>Front-End</summary>

- [vue](https://vuejs.org/)
- [HTML](https://www.w3schools.com/css/)
- [CSS](https://www.w3schools.com/css/)

</details>

<details>
<summary>Back-End</summary>

- [Java](https://www.java.com/pt-BR/?msclkid=7faa842eb8f811ecab39772d4c1ae90b)

- [Spring boot](https://spring.io/projects/spring-boot)

</details>

<details>
<summary>Database</summary>

- [Oracle Autonomous Database](https://www.oracle.com/autonomous-database/)
</details>

<details>
<summary>Meetings and Communication</summary>

- [Discord](https://discord.com/?msclkid=b4f5af84b8f811ecbd81c127a0ae68a7)

- [Whatsapp](https://www.whatsapp.com/)

- [Slack](https://slack.com/intl/pt-br/?msclkid=c00e628eb8f811ecaef374bb86d7f056)
</details>

<p align="right">(<a href="#top">Scroll to top</a>)</p>

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
