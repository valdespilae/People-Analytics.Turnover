# 📊Projeto de People Analytics: Redução do Turnover com CRISP-DM
 Projeto da formação "Gerando Valor com Dados" da Escola de Dados [Preditiva.IA](https://www.preditiva.ai.com)

## Índice
- [Project Overview](Project-overview)
- [Benchmark de Turnover no Setor de Tecnologia no Brasil](Benchmark-de-Turnover-no-Setor-de-Tecnologia-no-Brasil)
- [Metodologia - CRISP-DM](Metodologia-CRISP-DM)

## *Project Overview*

Este projeto tem como objetivo aplicar técnicas de análise de dados para entender os principais fatores que influenciam o turnover de funcionários em uma empresa de tecnologia. A abordagem segue a metodologia **CRISP-DM**, que é um padrão de mercado para projetos de Data Mining e Data Science.

## ✨ Benchmark de Turnover no Setor de Tecnologia no Brasil

Compreender a taxa de rotatividade (turnover) é essencial para contextualizar a situação da empresa analisada em relação ao mercado. Abaixo estão os principais dados de benchmark disponíveis para o setor de tecnologia no Brasil.

### 🔹 Visão Geral

- A média de rotatividade no Brasil ficou em **51%** entre abril de 2022 e maio de 2023, uma das mais altas do mundo.
- No setor de tecnologia, a taxa média de turnover foi de **13,2%**, a maior entre todos os setores avaliados.
- Em comparação global, é comum observar taxas entre **13% e 18% ao ano** no setor de tecnologia, podendo chegar a **25%** em startups.

### 🔹 Comparações e Dados Históricos

- Antes da pandemia (2019), o turnover médio no setor de TI no Brasil era de **39%**, enquanto a média geral era **41%**.
- Subsetores como desenvolvimento de software apresentavam taxas menores (33%–39%).
- Cargos executivos de tecnologia no Brasil apresentam turnover voluntário de **20%** e involuntário de **14%**, totalizando **34%**.

### 🔹 Segmentação por Subárea

- UX e Design: aproximadamente **23%**
- Engenheiros de Dados e Software: entre **21% e 22%**
- Suporte técnico e áreas de operação: **até 25%**

### ✅ Insight para o Projeto

Com base nesses dados, uma meta realista para a organização pode ser a redução da taxa de turnover para **abaixo de 15%**, posicionando-se entre os benchmarks mais estáveis do setor de tecnologia nacional e internacional.



---

## Metodologia - CRISP-DM

![image](https://github.com/user-attachments/assets/c5129457-0470-44cb-b0b2-cadf5b2de4fd)
*fonte:[https://towardsdatascience.com/using-crisp-dm-to-grow-as-data-scientist-a07ce3fd9d56/] (https://towardsdatascience.com/using-crisp-dm-to-grow-as-data-scientist-a07ce3fd9d56/)*

### 📘 1. Compreensão do Negócio (Business Understanding)

#### 🎯 Objetivo

Reduzir o turnover (rotatividade) dos funcionários por meio da análise de dados comportamentais, profissionais e demográficos dos colaboradores.

#### 🧩 Problema de Negócio

A alta rotatividade gera aumento de custos com recrutamento, perda de conhecimento institucional e impacto na produtividade. Identificar os principais fatores associados ao desligamento pode apoiar estratégias de retenção mais eficazes.

---

### 📗 2. Compreensão dos Dados (Data Understanding)

#### 🗃️ Fonte dos Dados

Base fictícia de Recursos Humanos com atributos relacionados aos funcionários.

#### 📊 Dicionário de Variáveis
Abaixo está a descrição das variáveis utilizadas no projeto, com sua classificação e faixas observadas:

| Variável                     | Descrição                                              | Classificação da Variável   | Intervalos ou faixas   |
|:-----------------------------|:-------------------------------------------------------|:----------------------------|:-----------------------|
| ID                           | Matrícula do funcionário                               | Quantitativa Discreta       | 1 - 1470               |
| Funcionário_deixou_a_empresa | Marcação sem funcionário deixou a empresa recentemente | Qualitativa Nominal         | Sim / Não              |
| Idade                        | Idade do funcionário                                   | Quantitativa Discreta       | 18-59 anos             |
| Frequência de Viagens        | Frequência de viagens a trabalho do funcionário        | Qualitativa Ordinal         | Não viaja; Viaja raramente; Viaja frequentemente|
| Distância_do_trabalho        | Distância em Km até o trabalho                         | Quantitativa Discreta       | 1 - 29 Km              |
> *A tabela completa com todas as variáveis analisadas neste caso estão anexadas ao projeto, dentro da pasta /docs/ no arquivo classificacao_variaveis.xlsx para consulta detalhada. *

#### 🎯 Variável Alvo

- `Funcionário_deixou_a_empresa` — Indica se o funcionário deixou a empresa recentemente (`1`) ou não (`0`).

#### 📌 Principais Variáveis Preditivas

- Idade  
- Salário  
- Frequência de viagens a trabalho  
- Distância até o trabalho  
- E-Sat (satisfação organizacional)  
- Equilíbrio de Vida  
- Horas extras  
- Anos no mesmo cargo  
- Tempo desde a última promoção  
- Tempo com o mesmo chefe  

#### 🔍 Ações realizadas

- Análise da estrutura da base de dados  
- Identificação dos tipos de variáveis (numéricas e categóricas)  
- Análise exploratória com gráficos, tabelas dinâmicas e estatísticas descritivas

---

### 📙 3. Preparação dos Dados (Data Preparation)

#### 🧹 Etapas da preparação

- Padronização dos nomes das colunas  
- Conversão de variáveis categóricas e numéricas  
- Tratamento de dados ausentes  
- Criação de variáveis derivadas (ex: anos desde última promoção)  

#### 🛠️ Ferramenta utilizada

- **Microsoft Excel** para limpeza, visualização e análise descritiva

---

### 📘 4. Modelagem (Modeling)

Neste projeto inicial, não foi utilizada modelagem estatística preditiva. O foco esteve em análises descritivas e exploratórias:

- Matriz de correlação para variáveis numéricas  
- Análise de associação entre variáveis categóricas e turnover  
- Gráficos e tabelas para identificar padrões visuais

> *Futuras versões do projeto podem aplicar regressão logística, árvore de decisão ou Random Forest.*

---

### 📕 5. Avaliação (Evaluation)

#### 📈 Resultados observados

- Maiores taxas de saída em funcionários com:
  - Baixa nota de equilíbrio de vida  
  - Baixa satisfação organizacional  
  - Longo tempo sem promoção  
  - Muitas horas extras  
  - Poucas horas de treinamento  

#### 🧠 Conclusão

Esses fatores servem como alerta para a área de Recursos Humanos priorizar ações preventivas e programas de retenção.

---

### 📓 6. Implantação (Deployment)

#### 📤 Entregáveis

- Dashboard em Excel com filtros e indicadores de turnover  
- Relatório com principais insights e recomendações para o RH  
- Documentação estruturada com base no CRISP-DM

#### 🗂️ Estrutura sugerida do repositório
---
## 📚 Referências

1. [IDC / LinkedIn — Panorama Turnover Brasil (2023)](https://br.linkedin.com/pulse/panorama-turnover-no-brasil-linkedin-news-brasil)
2. [Valor Econômico — Rotatividade no mercado de trabalho (2022)](https://valor.globo.com)
3. [CAGED / Ministério do Trabalho (2019–2023)](https://www.gov.br/trabalho-e-emprego)
4. [Mercer Brasil — Benchmarking executivo em TI (2023)](https://www.mercer.com.br)
5. [Tech Reh — Dados de rotatividade por cargo em tecnologia (2023)](https://www.techreh.com)
6. [Great Place to Work — Estudo de rotatividade em Startups (2022)](https://gptw.com.br)

