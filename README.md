<p align="center">
  <img src="https://github.com/user-attachments/assets/1e0540ec-e599-4f33-8eda-886dbe2eeccf" alt="Descrição da imagem">
</p>

# 📊Projeto People Analytics: Redução do Turnover com CRISP-DM
 Projeto da formação "Gerando Valor com Dados" da Escola de Dados [Preditiva.IA](https://www.preditiva.ai.com)

## Índice
- [Contextualização](Contextualização.)
   - [Benchmark de Turnover no Setor de Tecnologia no Brasil.](Benchmark-de-Turnover-no-Setor-de-Tecnologia-no-Brasil)
- [Metodologia:  CRISP-DM](Metodologia-CRISP-DM.)
  - [Etapa 1: Compreensão do Negócio -*Business Understanding*-.](Etapa-1-Compreensão-do-Negócio-Business-Understanding)
  - [Etapa 2: Compreensão dos Dados -*Data Understanding*-.](Etapa-2-Compreensão-dos-Dados-Data-Understanding)

## 📌 Contextualização  

### O desafio do ***turnover*** nas empresas  

O ***turnover*** ou **rotatividadedos funcionários**, é um dos desafios mais críticos enfrentados pelas empresas atualmente. Segundo um levantamento publicado em **agosto de 2023** pela consultoria **Robert Half**, o Brasil lidera o ranking global de rotatividade, com uma taxa de **56%**, colocando o país entre os que mais enfrentam desafios com retenção de talentos. Esse índice elevado reflete mudanças estruturais no mercado de trabalho, impulsionadas por transformações nas expectativas dos profissionais, que estão cada vez mais atentos ao propósito, à flexibilidade e ao equilíbrio entre vida pessoal e profissional[(1)](-1).

Outro estudo publicado pela **Evermonte** em **julho de 2024** apontou que **39% dos desligamentos no Brasil em 2023 foram voluntários**, ou seja, motivados pela decisão dos próprios colaboradores[(2)](-2). Esse dado reforça que fatores como satisfação profissional, oportunidades de crescimento e ambiente organizacional exercem influência direta na retenção de talentos, evidenciando a necessidade de estratégias mais humanas e personalizadas por parte das empresas.

### 🔎 Benchmark de ***Turnover*** no Setor de Tecnologia no Brasil  
Para contextualizar melhor este projeto, é essencial entender a taxa de rotatividade no setor de tecnologia e como a empresa analisada se compara ao mercado. 


### 📊 Visão Geral  

- A média de rotatividade no Brasil -área de tecnología-  ficou em **51%** entre abril de 2022 e maio de 2023, uma das mais altas do mundo[(3)](3) 
- No setor de tecnologia, a taxa média de turnover foi de **13,2%**, a maior entre todos os setores avaliados[(4)](4).  
- Em comparação global, é comum observar taxas entre **13% e 18% ao ano** no setor de tecnologia, podendo chegar a **25%** em startups[(5)](5).  

### 📈 Comparações e Dados Históricos  

° Antes da pandemia (2019), o turnover médio no setor de TI no Brasil era de **39%**, enquanto a média geral era **41%**[(6)](6).  
° Subsetores como desenvolvimento de software apresentavam taxas menores (**33%–39%**)[(6)](6).  
° Cargos executivos de tecnologia no Brasil apresentam turnover voluntário de **20%** e involuntário de **14%**, totalizando **34%**[(7)](7).  

### 🔍 Segmentação por Subárea  

- **UX e Design**: aproximadamente **23%**;  
- **Engenheiros de Dados e Software**: entre **21% e 22%**; 
- **Suporte técnico e áreas de operação**: **até 25%**[(8)](8). 

### 🎯 Insight para o Projeto  

Com base nesses dados, uma meta realista para a organização pode ser a redução da taxa de turnover para **abaixo de 15%**, posicionando-se entre os **benchmarks** mais estáveis do setor de tecnologia nacional e internacional. 

### Estratégias para minimizar o turnover  

Diante desse cenário, e com base às pesquesisas abordadas anteriormente, foram identificados estratégicas inovadores que as empresas precisam adotar para reduzir a rotatividade. Algumas abordagens incluem:  

- **Criar um ambiente de trabalho dinâmico**, onde os funcionários sintam que estão evoluindo constantemente.  
- **Investir em aprendizado contínuo**, incentivando o desenvolvimento profissional.  
- **Ouvir os colaboradores**, garantindo que suas necessidades e expectativas sejam atendidas.  

O ***turnover*** não é apenas uma questão de remuneração, mas sim de **propósito e engajamento**. Empresas que conseguem oferecer um ambiente estimulante e oportunidades de crescimento tendem a reter seus talentos por mais tempo.  

## Metodologia - CRISP-DM

### 🔎 O que é CRISP-DM?  

A metodologia ***CRISP-DM (Cross Industry Standard Process for Data Mining)*** é um modelo padrão amplamente utilizado para projetos de **Data Science** e **Machine Learning**. Criada nos anos 1990, essa abordagem orienta o processo de análise de dados em **seis fases estruturadas**, garantindo que cada etapa seja bem definida e alinhada aos objetivos do negócio.  

### 🚀 Por que utilizar CRISP-DM neste projeto?  

Este projeto busca **entender os fatores que influenciam o turnover** e propor **estratégias para reduzir a rotatividade** dos funcionários em uma empresa de tecnologia. Como se trata de uma análise exploratória e investigativa, a CRISP-DM é a metodologia ideal, pois oferece um fluxo de trabalho lógico e sistemático para abordar o problema de forma eficiente.  

<p align="center">
<img src="https://github.com/user-attachments/assets/c5129457-0470-44cb-b0b2-cadf5b2de4fd" alt="Descrição da imagem" width="500" height="500">
</p>

*fonte: [ https://towardsdatascience.com/using-crisp-dm-to-grow-as-data-scientist-a07ce3fd9d56/]( https://towardsdatascience.com/using-crisp-dm-to-grow-as-data-scientist-a07ce3fd9d56/)*

### 🔬 As seis fases do CRISP-DM e sua aplicação no projeto  

1. **Compreensão do Negócio**  
   - Definição do problema: Quais fatores influenciam a saída dos funcionários?  
   - Análise dos objetivos da empresa para reduzir o turnover.  

2. **Compreensão dos Dados**  
   - Exploração do conjunto de dados fornecido pelo RH.  
   - Identificação de variáveis relevantes e possíveis padrões.  

3. **Preparação dos Dados**  
   - Limpeza e organização dos dados para análise.  
   - Conversão de variáveis qualitativas em numéricas, se necessário.  

4. **Modelagem**  
   - Aplicação de técnicas estatísticas para entender correlações entre as variáveis.  
   - Avaliação da relação entre turnover e fatores internos da empresa.  

5. **Avaliação**  
   - Interpretação dos resultados obtidos na modelagem.  
   - Comparação com benchmarks do setor para validar insights.  

6. **Implementação e Monitoramento**  
   - Recomendação de políticas para reduzir o turnover.  
   - Definição de métricas para acompanhamento da retenção dos funcionários.  

### 📈 Benefícios da CRISP-DM para este estudo  

✔ **Estruturação clara do processo de análise**  
✔ **Maior confiabilidade nos resultados obtidos**  
✔ **Facilidade na comunicação dos insights ao RH e gestores**  
✔ **Melhor alinhamento entre dados e tomada de decisão**  

Com essa metodologia, garantimos que o projeto será conduzido de forma **organizada, eficiente e baseada em evidências**, trazendo insights valiosos para reduzir o turnover na empresa de tecnologia.  

## Metodologia - CRISP-DM. Framework de Análise de Dados. 

## 📘 Etapa 1: Compreensão do Negócio (Business Understanding)

Para compreender quais são as características que fazem um funcionário ficar ou deixar a empresa de Tecnologia, o departamento de Recursos Humanos da empresa catalogou informações de **1.470 funcionários** que 
deixaram ou permaneceram na companhia no *último ano*. O resultado desse levantamento gerou **19 possíveis fatores** para tentar explicar o comportamento do ***turnover***. Para conhecer esses fatores, verifique a tabela de metadados
existentes na secção seguinte ou na pasta */docs/* no arquivo .xlsx *classificação_variaveis_turnover*

#### ✅ Objetivo do projeto:
- **Reduzir** o ***turnover*** e **melhorar a retenção dos funcionários** meio da análise de dados comportamentais, profissionais e demográficos dos colaboradores.
- **Identificar** quais **fatores** mais influenciam a saída dos colaboradores.
- **Criar um plano de ação** *5W2H* baseado nos insights obtidos, propondo estratégias para minimizar a rotatividade.

#### ✅ Impacto do turnover:
- Custos elevados com recrutamento e treinamento.
- Perda de produtividade e conhecimento institucional.
- Impacto na cultura e no clima organizacional.

#### ✅ Variáveis que podem explicar o turnover:
- Dados demográficos (*idade, gênero, estado civil*).
- Características do trabalho (*salário, equilíbrio entre vida pessoal e profissional*).
- Ambiente corporativo (*satisfação organizacional, relação com o chefe*).
- Histórico do funcionário (*tempo de empresa, promoção, mudanças de cargo*).
  
#### ✅ Perguntas estratégicas para investigação:
- *Quais políticas/fatores da empresa deveriam mudar de forma a minimizar o turnover*
- *O turnover é maior em algum grupo específico de funcionários?*
- *Existe correlação entre salário, tempo de empresa e saída voluntária?*
- *Como o clima organizacional impacta a retenção dos talentos?*
- *Funcionários que viajam frequentemente são mais propensos a sair?*

---

### 🔍 Etapa 2: Compreensão dos Dados (Data Understanding)


Após a definição clara do problema de negócio e dos objetivos estratégicos do projeto, o próximo passo consiste em explorar a base de dados fornecida pelo departamento de Recursos Humanos. Para isso, foi disponibilizado um arquivo no formato **.xlsx**, contendo informações de **1.470 funcionários** que permaneceram ou deixaram a empresa no último ano. A base contempla variáveis de diferentes naturezas — **demográficas, funcionais e comportamentais** — que foram organizadas e documentadas na tabela de **metadados**, facilitando a identificação e classificação de cada atributo. Ao todo, foram listadas **19 variáveis potencialmente associadas ao turnover**, como idade, salário, tempo na empresa, frequência de viagens, satisfação organizacional, entre outros fatores. 

O objetivo para esta etapa é **a compreensão de cada variavel, sua distribuição, e a identificação de variáveis relevantes com o ***turnover*** e a detecção de outliers**. Para ello, faremos uso da **Análise Exploratória de Dados (AED)** [(9)](9) como abordgem fudamental na ciência e análeses de dados por meio da ferramenta Microsoft Excel 365®. Além disso, durante esta etapa, e antes do *AED*, é crucial verificar a qualidade dos dados, por meio do chamado *Sanity Check*, permitindo identificar valores fora de faixas plausíveis (outliers), anomalias ou registros possivelmente inconsistentes. 

### 🧰 Principais Técnicas Utilizadas nesta Etapa

- **Tabelas de Frequência**  
  Construção de frequências **absolutas**, **relativas** e **acumuladas** para as variáveis qualitativas, como Gênero, Estado Civil, Formação e Frequência de Viagens.

- **Visualizações Gráficas**  
  Uso de **Box-plots**, **Histogramas** e **Gráficos de Barras ou Colunas**, para identificar padrões visuais e outliers em variáveis quantitativas como Salário, Idade e Tempo na Empresa.

- **Medidas Resumo**  
  Cálculo de estatísticas descritivas como:
  - **Média**
  - **Mediana**
  - **Quartis**
  - **Desvio Padrão**
  - **Mínimos e máximos**

- **Análise Bidimensional**  
  Avaliação da associação entre o turnover e outras variáveis por meio de:
  - **Correlação de Pearson** (para variáveis quantitativas)
  - **Coeficiente de Determinação (R²)**
  - **Information Value (IV)** para medir o poder explicativo das variáveis em relação à saída dos funcionários.

Essas análises oferecem a base necessária para a próxima etapa do projeto — a preparação dos dados e construção de modelos que ajudem a identificar os fatores mais relevantes associados ao turnover.


#### 📊 Dicionário de Dados

Abaixo está a descrição das variáveis utilizadas no projeto, com sua classificação e possíveis faixas observadas:
  
 Tabela 1. Dicionário de Dados (**Metadados**)

| **Variável**                  | **Descrição**                                                         |**Classificação da Variável**|**Intervalos ou faixas**|
|:------------------------------|:----------------------------------------------------------------------|:----------------------------|:--------------------------------------------------------|
| ID                            | Matrícula do funcionário                                              | Qualitativa Discreta        | 1 - 1.470                                                |
| Funcionário_deixou_a_empresa  | Marcação se o funcionário deixou a empresa recentemente               | Qualitativa Nominal         | Sim / Não                                               |
| Idade                         | Idade do funcionário                                                  | Quantitativa Discreta       | 18-59 anos                                              |
| Frequência de Viagens         | Frequência de viagens a trabalho do funcionário                       | Qualitativa Ordinal         | Não viaja, Viaja raramente, Viaja frequentemente        |
| Distância_do_trabalho         | Distância em Km até o trabalho                                        | Quantitativa Discreta       | 1 - 29 Km                                               |
| Formação                      | Nível de formação                                                     | Qualitativa Ordinal         | Ensino Médio, Ensino Técnico, Mestrado, Superior, Doutorado |
| E-Sat                         | Satisfação com o clima organizacional                                 | Qualitativa Ordinal         | Baixo, Médio, Alto, Muito Alto                         |
| Gênero                        | Gênero do funcionário                                                 | Qualitativa Nominal         | H: Masculino; F: Feminino                              |
| Estado_Civil                  | Estado civil do funcionário                                           | Qualitativa Nominal         | Solteiro, Casado, Divorciado                           |
| Salário                       | Salário mensal                                                        | Quantitativa Contínua       | R$ 1.009,00 - R$ 19.999,00                              |
| Qte_Empresas_Trabalhadas      | Quantidade de empresas que o funcionário já trabalhou                 | Quantitativa Discreta       | 0 - 9                                                   |
| Faz_hora_extras?              | Se o funcionário costuma fazer hora extra                             | Qualitativa Nominal         | Sim / Não                                               |
| Perc_de_aumento               | Percentual de aumento de salário de 2018 a 2019                       | Quantitativa Contínua       | 11% - 25%                                               |
| Qte_ações_da_empresa          | Quantidade de lotes de ações da empresa que o funcionário possui      | Quantitativa Discreta       | 0 - 3                                                   |
| Tempo_de_carreira (Anos)      | Tempo em anos que o funcionário tem de carreira                       | Quantitativa Discreta       | 0 - 40 anos                                             |
| Horas_de_treinamento          | Quantidade de horas de treinamento no último ano                      | Quantitativa Discreta       | 0 - 6 horas                                             |
| Equilibrio_de_Vida            | Nota sobre equilíbrio entre vida pessoal e profissional               | Qualitativa Ordinal         | Ruim, Bom, Muito bom, Excelente                        |
| Tempo_de_empresa (Anos)       | Tempo em anos que o funcionário trabalha na empresa                   | Quantitativa Discreta       | 0 - 40 anos                                             |
| Anos_no_mesmo_cargo           | Tempo em anos que o funcionário atua no mesmo cargo                   | Quantitativa Discreta       | 0 - 18 anos                                             |
| Anos_desde_a_ultima_promocao  | Tempo em anos desde a última promoção                                 | Quantitativa Discreta       | 0 - 15 anos                                             |
| Anos_com_o_mesmo_chefe        | Tempo em anos que responde ao mesmo chefe                             | Quantitativa Discreta       | 0 - 17 anos                                             |


#### 🎯 Variável Alvo

- `Funcionário_deixou_a_empresa` — Indica se o funcionário deixou a empresa recentemente (`1`) ou não (`0`).


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
## 📌 Referências  

[^1]: ROBERT HALF. *Brasil lidera índice de rotatividade de funcionários em todo o mundo: 56%*. Publicado em 23 ago. 2023. Disponível em: [https://www.panrotas.com.br/100xbrasil/pesquisas-e-estatisticas/2023/08/brasil-lidera-indice-de-rotatividade-de-funcionarios-em-todo-o-mundo-56_199128.html](https://www.panrotas.com.br/100xbrasil/pesquisas-e-estatisticas/2023/08/brasil-lidera-indice-de-rotatividade-de-funcionarios-em-todo-o-mundo-56_199128.html)

[^2]: EVERMONTE. *Turnover: por que os colaboradores estão permanecendo menos tempo nas companhias?*. Publicado em 08 jul. 2024. Disponível em: [https://evermonte.com/turnover-por-que-os-colaboradores-estao-permanecendo-menos-tempo-nas-companhias-evermonte-headhunter](https://evermonte.com/turnover-por-que-os-colaboradores-estao-permanecendo-menos-tempo-nas-companhias-evermonte-headhunter)

[^3]: MUNDO RH. *Retenção de talentos e baixa rotatividade são fundamentais para o crescimento do setor de tecnologia no Brasil*. Publicado em 16 abr. 2024. Disponível em: [https://www.mundorh.com.br/retencao-de-talentos-e-baixa-rotatividade-sao-fundamentais-para-o-crescimento-do-setor-de-tecnologia-no-brasil](https://www.mundorh.com.br/retencao-de-talentos-e-baixa-rotatividade-sao-fundamentais-para-o-crescimento-do-setor-de-tecnologia-no-brasil)

[^4]:  GUPY. *Retenção de talentos de vagas com alto turnover: como fazer*. Publicado em 26 fev. 2020. Disponível em: [https://www.gupy.io/blog/retencao-de-talentos-turnover](https://www.gupy.io/blog/retencao-de-talentos-turnover)

[^5]: LINKEDIN TALENT SOLUTIONS. *Global Talent Trends Report 2022*. Disponível em: [https://business.linkedin.com/talent-solutions/resources/talent-strategy/global-talent-trends-report](https://business.linkedin.com/talent-solutions/resources/talent-strategy/global-talent-trends-report)

[^6]: TI INSIDE. *Setor de TI apresentava índices menores de rotatividade antes da pandemia, aponta relatório*. Publicado em 18 out. 2022. Disponível em: [https://tiinside.com.br/18/10/2022/setor-de-ti-apresentava-indices-menores-de-rotatividade-antes-da-pandemia-aponta-relatorio](https://tiinside.com.br/18/10/2022/setor-de-ti-apresentava-indices-menores-de-rotatividade-antes-da-pandemia-aponta-relatorio)

[^7]: FORBES BRASIL. *Empresas mexem no C-level para adaptar-se aos novos tempos*. Publicado em 9 nov. 2022. Disponível em: [https://forbes.com.br/carreira/2022/11/empresas-mexem-no-c-level-para-adaptar-se-aos-novos-tempos](https://forbes.com.br/carreira/2022/11/empresas-mexem-no-c-level-para-adaptar-se-aos-novos-tempos)

[^8]: G1 — Pós PUCPR Digital. *Turnover: o índice de rotatividade que vem impactando as empresas*. Publicado em 3 dez. 2022. Disponível em: [https://g1.globo.com/pr/parana/especial-publicitario/pos-pucpr-digital/voce-no-futuro/noticia/2022/12/03/turnover-o-indice-de-rotatividade-que-vem-impactando-as-empresas.ghtml](https://g1.globo.com/pr/parana/especial-publicitario/pos-pucpr-digital/voce-no-futuro/noticia/2022/12/03/turnover-o-indice-de-rotatividade-que-vem-impactando-as-empresas.ghtml)

[^9]: ESTATÍSTICA FÁCIL. *O que é: Análise Exploratória de Dados*. Disponível em: [https://estatisticafacil.org/glossario/o-que-e-analise-exploratoria-de-dados/](https://estatisticafacil.org/glossario/o-que-e-analise-exploratoria-de-dados/)

 
