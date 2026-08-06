# Painel-Executivo-de-Contratos
Solução de Business Intelligence para acompanhamento da execução de contratos administrativos, consolidando indicadores operacionais e executivos em um modelo analítico único.
# Gestão de Contratos — Business Intelligence

Uma solução de Business Intelligence desenvolvida para consolidar informações de contratos administrativos em um modelo analítico único, transformando dados dispersos em indicadores para apoio à tomada de decisão.

Este repositório documenta a arquitetura, a modelagem e as principais decisões técnicas do projeto. O código-fonte não é disponibilizado.

---

# Sobre o projeto

A gestão de contratos administrativos envolve dezenas de informações distribuídas entre planilhas, documentos e controles paralelos. Embora os dados existissem, responder perguntas simples exigia consultas manuais, cruzamento de arquivos e conhecimento operacional da equipe.

Este projeto nasceu da necessidade de organizar essas informações em um modelo único, permitindo acompanhamento contínuo da execução contratual, prazos, reajustes, notificações, termos aditivos e pagamentos.

Mais do que construir um dashboard, o objetivo foi estruturar uma base analítica confiável que pudesse servir como fonte única de informação para consultas operacionais e indicadores gerenciais.

---

# Meu papel

Neste projeto atuei desde a identificação do problema até a entrega da solução.

As principais atividades envolveram:

- levantamento das regras de negócio junto às áreas responsáveis;
- consolidação de diversas bases de dados;
- definição da arquitetura do modelo analítico;
- modelagem dos relacionamentos;
- construção das transformações em Power Query;
- desenvolvimento das medidas em DAX;
- criação dos dashboards executivos e operacionais;
- validação dos indicadores junto aos usuários.

O foco sempre foi utilizar tecnologia para reduzir trabalho manual e melhorar a qualidade das informações disponíveis para a gestão.

---

# O problema

Antes da implantação, o acompanhamento contratual dependia de diversas planilhas independentes contendo informações sobre:

- contratos;
- prazos;
- reajustes;
- termos;
- notificações;
- pagamentos;
- dados cadastrais.

Cada consulta exigia cruzamentos manuais entre arquivos diferentes, tornando a atualização lenta e sujeita a inconsistências.

---

# A solução

Foi desenvolvido um modelo analítico centralizado capaz de consolidar todas essas informações em um único ambiente.

A partir dessa estrutura tornou-se possível acompanhar:

- contratos vigentes;
- prazos críticos;
- reajustes concedidos;
- prorrogações;
- notificações emitidas;
- histórico contratual;
- pagamentos realizados;
- indicadores executivos.

Toda a atualização do modelo foi desenhada para exigir o mínimo possível de intervenção manual.

---

# Arquitetura dos dados

O modelo foi estruturado tendo a tabela **BASE CONTRATOS** como entidade central, responsável por concentrar as informações cadastrais dos contratos e estabelecer relacionamento com as demais entidades do processo.

O objetivo foi representar o ciclo de vida da gestão contratual de forma integrada, permitindo consultas operacionais e análises gerenciais a partir de uma única base de dados.

Principais componentes do modelo:

- Base Contratos (entidade central)
- Dados Cadastrais
- Pagamentos
- Prazos
- Reajustes
- Prorrogações
- Termos
- Notificações
- Dimensão de Datas
- Tipo de Movimentação

As medidas DAX foram organizadas em uma tabela exclusiva, facilitando manutenção, reutilização e padronização dos indicadores utilizados pelos dashboards.

---

# Modelagem

A figura abaixo apresenta a estrutura lógica do modelo analítico desenvolvido para consolidar as diferentes informações relacionadas à gestão contratual.

![Modelagem do Modelo Analítico](screenshots/modelagem-contratos.png)

A modelagem foi construída priorizando a organização das entidades de negócio e seus relacionamentos, permitindo consolidar informações provenientes de diferentes controles em um único ambiente analítico.

Embora este projeto tenha sido desenvolvido antes do aprofundamento dos meus estudos em modelagem dimensional durante o MBA em Data Science e Analytics, ele representou um importante passo na minha evolução em Business Intelligence.

Se fosse iniciado hoje, algumas decisões de modelagem seriam diferentes, especialmente na organização entre fatos e dimensões compartilhadas. Ainda assim, a estrutura adotada cumpriu plenamente seu objetivo de oferecer uma base consistente para análise da execução contratual e serviu como fundamento para projetos posteriores de maior complexidade.

---

# Principais funcionalidades

- Consolidação de múltiplas bases de dados.
- Atualização simplificada do modelo analítico.
- Indicadores executivos.
- Consultas operacionais self-service.
- Acompanhamento de prazos contratuais.
- Controle de reajustes e prorrogações.
- Histórico contratual consolidado.
- Navegação por filtros cruzados.
- Modelo preparado para evolução contínua.

---

# Tecnologias

- Power BI
- Power Query (M)
- DAX
- Modelagem de Dados
- Excel
- Business Intelligence

---

# Resultados

A solução passou a ser utilizada como ferramenta diária de acompanhamento da execução contratual, reduzindo significativamente consultas manuais e aumentando a confiabilidade das informações utilizadas pela equipe gestora.

Além da melhoria operacional, o projeto criou uma base estruturada que permitiu a evolução para outras iniciativas de automação e gestão de dados.

---

# Aprendizados Técnicos

Este projeto marcou minha transição de um uso mais operacional do Power BI para uma abordagem baseada em modelagem de dados.

Foi a partir dele que aprofundei conceitos como:

- modelagem de dados;
- organização de medidas DAX;
- relacionamentos entre tabelas;
- separação entre camada de dados e camada analítica;
- construção de soluções self-service para apoio à decisão.

Grande parte desses aprendizados foi posteriormente aplicada em projetos de automação de processos e desenvolvimento de sistemas utilizando Python, Django e PostgreSQL.

Hoje eu provavelmente faria algumas escolhas arquiteturais diferentes, especialmente na organização do modelo dimensional. Mantive essa versão documentada porque ela representa fielmente a evolução do projeto e demonstra como meu entendimento sobre modelagem de dados amadureceu ao longo do tempo.

---

# Dashboard

O dashboard público pode ser acessado em:

https://app.powerbi.com/view?r=eyJrIjoiYzYxNDdjMWUtOWJjNC00YmY0LWI5MmUtMjA5MjAzOGVhNTE3IiwidCI6IjNhNzhiMGNkLTdjOGUtNDkyOS04M2Q1LTE5MGE2Y2MwMTM2NSJ9
