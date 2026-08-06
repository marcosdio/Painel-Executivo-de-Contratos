# Painel-Executivo-de-Contratos
Solução de Business Intelligence para acompanhamento da execução de contratos administrativos, consolidando indicadores operacionais e executivos em um modelo analítico único.
# Gestão de Contratos — Business Intelligence

Uma solução de Business Intelligence desenvolvida para consolidar informações de contratos administrativos em um modelo analítico único, transformando dados dispersos em indicadores para apoio à tomada de decisão.

Este repositório documenta a arquitetura, a modelagem e as decisões técnicas do projeto. O código-fonte não é disponibilizado.

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
- modelagem dimensional;
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

O modelo foi estruturado tendo a tabela **BASE CONTRATOS** como entidade central, relacionando-se às demais tabelas de negócio.

Principais componentes do modelo:

- Base Contratos
- Dados Cadastrais
- Pagamentos
- Prazos
- Reajustes
- Prorrogações
- Termos
- Notificações
- Calendário
- Tabela de Medidas

As métricas foram centralizadas em uma tabela exclusiva de medidas, facilitando manutenção, organização e reutilização.

---

# Modelagem

![Modelagem do modelo analítico](screenshots/Captura%20de%20tela%202026-08-05%20234016.png)

A modelagem foi construída buscando reduzir redundâncias, preservar integridade dos dados e facilitar a criação de indicadores.

Embora tenha sido desenvolvida antes do aprofundamento em modelagem dimensional realizado posteriormente durante meu MBA em Data Science e Analytics, muitos dos conceitos adotados permanecem válidos e serviram como base para projetos posteriores.

---

# Principais funcionalidades

- Consolidação de múltiplas bases de dados.
- Atualização automatizada do modelo.
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
- Modelagem Dimensional
- Excel
- Business Intelligence

---

# Resultados

A solução passou a ser utilizada como ferramenta diária de acompanhamento da execução contratual, reduzindo significativamente consultas manuais e aumentando a confiabilidade das informações utilizadas pela equipe gestora.

Além da melhoria operacional, o projeto criou uma base estruturada que permitiu a evolução para outras iniciativas de automação e gestão de dados.

---

# Lições aprendidas

Este foi um dos projetos que consolidou minha transição da gestão financeira tradicional para uma atuação mais voltada à análise de dados.

O desenvolvimento dessa solução reforçou alguns princípios que continuam presentes nos meus projetos atuais:

- antes de construir dashboards, é necessário organizar os dados;
- um bom modelo analítico vale mais do que dezenas de gráficos;
- tecnologia gera valor quando reduz trabalho manual e melhora a tomada de decisão;
- compreender profundamente as regras de negócio é tão importante quanto dominar a ferramenta.

Esses aprendizados serviram como base para projetos posteriores envolvendo automação de processos, desenvolvimento de aplicações e utilização de Inteligência Artificial aplicada à gestão pública.

---

# Dashboard

O dashboard público pode ser acessado em:

**https://app.powerbi.com/view?r=eyJrIjoiYzYxNDdjMWUtOWJjNC00YmY0LWI5MmUtMjA5MjAzOGVhNTE3IiwidCI6IjNhNzhiMGNkLTdjOGUtNDkyOS04M2Q1LTE5MGE2Y2MwMTM2NSJ9**
