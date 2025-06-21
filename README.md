<p align="center">
  <img src="https://github.com/user-attachments/assets/1e0540ec-e599-4f33-8eda-886dbe2eeccf" alt="Descrição da imagem">
</p>

# 📊Projeto People Analytics: Redução do Turnover com CRISP-DM
 Projeto da formação "Gerando Valor com Dados" da Escola de Dados [Preditiva.IA](https://www.preditiva.ai.com)

## Índice
- [Contextualização](#-contextualização)
   - [Benchmark de Turnover no Setor de Tecnologia no Brasil.](#-benchmark-de-turnover-no-setor-de-tecnologia-no-brasil)
- [Metodologia: CRISP-DM](#-metodologia-crisp-dm)
  - [Etapa 1: Compreensão do Negócio -*Business Understanding*-.](#-etapa-1-compreensão-do-negócio-business-understanding)
  - [Etapa 2: Compreensão dos Dados -*Data Understanding*-.](#-etapa-2-compreensão-dos-dados-data-understanding)

## 📌 Contextualização  

### O desafio do ***turnover*** nas empresas  

O ***turnover*** ou **rotatividadedos funcionários**, é um dos desafios mais críticos enfrentados pelas empresas atualmente. Segundo um levantamento publicado em **agosto de 2023** pela consultoria **Robert Half**, o Brasil lidera o ranking global de rotatividade, com uma taxa de **56%**, colocando o país entre os que mais enfrentam desafios com retenção de talentos. Esse índice elevado reflete mudanças estruturais no mercado de trabalho, impulsionadas por transformações nas expectativas dos profissionais, que estão cada vez mais atentos ao propósito, à flexibilidade e ao equilíbrio entre vida pessoal e profissional [(1)](-1).

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

<div align="center">
  <img src="https://github.com/user-attachments/assets/c5129457-0470-44cb-b0b2-cadf5b2de4fd" alt="Box plot dos salários" width="500" height="500"/>
  <p><strong>Figura 1:</strong> Modelo de processo CRISP-DM</p>
  <p style="font-size: 0.9em;">
    <em>Fonte:</em> TOWARDS DATA SCIENCE. <strong>Using CRISP-DM to Grow as a Data Scientist</strong>. Publicado em 2 abr. 2020.
    Disponível em: <a href="https://towardsdatascience.com/using-crisp-dm-to-grow-as-data-scientist-a07ce3fd9d56" target="_blank">https://towardsdatascience.com/...</a>
  </p>
</div>

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

O objetivo para esta etapa é **a compreensão de cada variavel, sua distribuição, e a identificação de variáveis relevantes com o ***turnover*** e a detecção de outliers**. Para ello, faremos uso da **Análise Exploratória de Dados (AED)** [(10)](10) como abordagem fundamental na ciência e análesis de dados por meio da ferramenta *Microsoft Excel®*. Além disso, durante esta etapa, e antes do *AED*, é crucial verificar a qualidade dos dados, por meio do chamado *Sanity Check*, permitindo identificar valores fora de faixas plausíveis -*outliers*-, anomalias ou registros possivelmente inconsistentes. 

### 🧰 Principais Técnicas Utilizadas nesta Etapa

- **Tabelas de Frequência**  
  Construção de frequências **absolutas**, **relativas** e **acumuladas** para as variáveis qualitativas, como Gênero, Estado Civil, Formação e Frequência de Viagens.

- **Visualizações Gráficas**  
  Uso de **Box-plots**, **Histogramas** e **Gráficos de Barras ou Colunas**, para identificar padrões visuais e outliers em todas as variáveis.

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
| *Funcionário_deixou_a_empresa*| Marcação se o funcionário deixou a empresa recentemente               | Qualitativa Nominal         | Sim / Não                                               |
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

#### Análises Univariada. Variáveis Qualitativas Nominal

##### Variável - Gênero do funcionário

<div align="center">
<img src= https://github.com/user-attachments/assets/eee1ae8c-0f07-417d-8b76-c9b59b04719e
  alt="Fig. Distribuição de gênero dos funcionário entrevistados" width="500" height="300">
  <p><strong> Figura 2:</strong> Distribuição dos funcionários da empresa por genero: M(Mulheres) e H(Homens)</p>
</div> 


🔑**Interpretações e reflexões:**
- **Distribuição equilibrada (mas levemente concentrada)**:
A equipe é composta por **60% de homens e 40% de mulheres**, o que mostra um certo equilíbrio, especialmente em comparação com a média de representatividade feminina no setor de tecnologia, que tende a ser mais baixa.
- **Ponto de atenção para a diversidade**:
Embora não haja um desequilíbrio alarmante, essa divisão pode servir como referência para **metas de inclusão e diversidade de gênero** dentro da organização, especialmente se refletir também em cargos de liderança e acesso a promoções.
- **Base para análises comparativas**:
Esse recorte será útil para verificar se há **diferenças significativas de turnover entre os gêneros**. Por exemplo:
- *A proporção de mulheres que se desligaram foi superior à de homens?*
- *O tempo médio de permanência é diferente entre os gêneros?* Infelizmente, esta questão não tem como ser abordada com as informações fornecidas pela empresa, porém, seria de suma importância contar com esses datos para futuras analises sobre o índice de *turnover* 
- Potencial para cruzamento com salário ou promoção:
Vale cruzar esse dado com outras variáveis como faixa salarial, número de promoções e satisfação no trabalho — é possível detectar, por exemplo, se há disparidades de gênero na remuneração ou reconhecimento.

##### Variável - Estado Civil

<div align="center">
<img src= https://github.com/user-attachments/assets/003955f8-39e3-46b1-9916-b594dc1776ef
  alt="Fig. Distribuição dos funcionários por Estado Civil" width="500" height="300">
  <p><strong> Figura 3:</strong> Distribuição dos funcionários por Estado Civil.</p>
</div> 

🔑**Interpretações e reflexões:**
- **Predomínio de funcionários casados**: A maior parte da força de trabalho é casada (**45,8%**), o que pode indicar maior estabilidade, mas também maior responsabilidade financeira, familiar e demanda por equilíbrio vida-trabalho.
- **Perfil jovem-adulto em destaque:** A soma de **solteiros (32%) + divorciados (22,2%)** representa mais de **54% da amostra**, o que sugere um público majoritariamente com perfil de transição de carreira, mobilidade geográfica ou em busca de desenvolvimento profissional acelerado.
- Possível relação com o turnover: Funcionários solteiros ou divorciados, por estarem em fases de maior flexibilidade pessoal, podem apresentar maior propensão à rotatividade. Isso será especialmente importante ao cruzar com a variável “Deixou a empresa”.
- Atenção para políticas personalizadas: Esses dados servem como base para refletir sobre programas de retenção mais segmentados. Por exemplo, casados podem valorizar benefícios familiares ou flexibilidade de horários, enquanto solteiros podem se interessar mais por trilhas de crescimento e mobilidade interna

##### Variável - Funcionário costuma fazer horas extras? Sim/Não


<div align="center">
<img src= https://github.com/user-attachments/assets/1a860244-9a10-4102-93fd-b1563b599d36
  alt="Fig. Distribuição dos funcionários por Estado Civil" width="500" height="300">
  <p><strong> Figura 4:</strong> Proporção de Funcionários que Realizam Horas Extras.</p>
</div> 


🔑*Interpretações e reflexões:*
- **A maioria dos colaboradores (71,7%) não realiza horas extras**, o que pode indicar um bom controle da carga de trabalho ou políticas eficazes de equilíbrio.
- **Quase 1 em cada 3 colaboradores faz horas extras (28,3%)** — esse grupo merece atenção especial, pois horas extras frequentes podem estar relacionadas a:
  - Sobrecarga de demandas em determinadas áreas;
  - Dificuldades de dimensionamento da equipe;
  - Potenciais gatilhos para rotatividade, principalmente se o esforço não estiver sendo compensado financeiramente ou reconhecido institucionalmente.
- Próximo passo interessante: Cruzar essa variável com: 
  - Turnover: Quem faz horas extras tem maior taxa de saída?
  - Satisfação no trabalho: Há correlação negativa?
  - Cargo ou área de atuação: As horas extras estão concentradas em setores específicos

#### Análises Univariada. Variáveis Qualitativas Ordinal
##### Variável - Frequência de Viagens

<div align="center">
<img src= https://github.com/user-attachments/assets/75be9dcc-fcd3-4a6a-a353-600743195316
  alt="Fig. Frequência de Viagens" width="500" height="400">
  <p><strong> Figura 5:</strong> Distribuição de Funcionários por Frequência de Viagens.</p>
</div> 


🔑*Interpretações e reflexões:*
- A maior parte dos colaboradores (**71%**) viaja raramente, sugerindo que a empresa adota um modelo com deslocamentos pontuais, talvez mais comum em funções técnicas ou administrativas.
- Quase 19% viaja com frequência, o que pode indicar funções voltadas à área comercial, suporte externo ou cargos executivos — esses colaboradores podem estar mais expostos a fatores de estresse, desequilíbrio vida-trabalho e potencial desgaste, especialmente se não houver compensações compatíveis.
- Apenas **10,2%** não viajam nunca, o que pode incluir funções exclusivamente internas, como suporte local, administrativo, ou posições mais júnior.
- Essa variável é forte candidata para durante a fase de Análesis bidimensional realizar uma análise de forma cruzada com:
  - Turnover: *Pessoas que viajam frequentemente deixam mais a empresa?*
  - Satisfação no trabalho: *Há correlação com baixa satisfação?*
  - Cargos: *Quem são os profissionais que mais se deslocam?*

##### Variável - 🎓 Formação Acadêmica

<div align="center">
<img src= https://github.com/user-attachments/assets/5d48e22e-5712-481b-a3bd-39164a9f6d63
  alt="Fig. Formação Acadêmica" width="500" height="300">
  <p><strong> Figura 6:</strong> Distribuição de Funcionários por Nível de Formação Acadêmica.</p>
</div> 

🔑*Interpretações e reflexões:*

- **Alta escolaridade da força de trabalho:** Cerca de **69% dos colaboradores possuem Ensino Superior ou Pós-Graduação (Mestrado/Doutorado)**. Isso sugere que a empresa opera em um contexto técnico ou altamente qualificado — possivelmente setores como tecnologia, pesquisa, engenharia ou serviços especializados.
- **Pico em Ensino Superior:** A maior parte está concentrada no Ensino Superior **(38,9%)**, seguido de Mestrado **(27,1%)**, o que indica **forte cultura de qualificação acadêmica** e uma provável valorização de títulos na progressão de carreira.
- **Baixa presença de Ensino Médio:** Apenas **11,6%** têm formação média, o que pode representar cargos operacionais ou de apoio com menor exigência técnica. Isso pode impactar o perfil de turnover nesses grupos (por exemplo: maior rotatividade por remuneração ou oportunidades externas).
- Doutorado é minoria, mas relevante: Com 48 pessoas **(3,3%)**, essa faixa pode representar áreas de inovação, pesquisa ou liderança técnica. Esses profissionais tendem a ter expectativas mais elevadas de desafios, autonomia e reconhecimento.

💡Potencial de Cruzamentos
Essa variável pode ser extremamente reveladora quando cruzada com:
- Salário Mensal: *Há proporcionalidade entre formação e remuneração?*
- Turnover: *Profissionais com maior formação estão deixando a empresa mais ou menos?*
- Promoção / Crescimento na empresa: *Qual o impacto da formação na trajetória interna?*

##### Variável - 🌤️ Satisfação com o Clima Organizacional

<div align="center">
<img src= https://github.com/user-attachments/assets/0977b81f-8d37-47ac-bf00-f323e20df4ce
  alt="Satisfação com o Clima Organizacional" width="500" height="300">
  <p><strong> Figura 7:</strong> Satisfação com o Clima Organizacional.</p>
</div> 

🔑*Interpretações e reflexões:*
Esta variável é altamente relevante para prever engajamento, produtividade e riscos de desligamento.
- **Clima amplamente positivo:** Quase **61% dos colaboradores** relataram níveis de satisfação **"Alto"** ou **"Muito Alto"**. Isso demonstra um ambiente organizacional saudável e colaborativo — uma excelente base para retenção e desempenho.
- **Dois polos bem definidos:** Enquanto boa parte demonstra alta satisfação, há um bloco expressivo de colaboradores (**38,8%**) com níveis **"Baixo"** ou **"Médio"**. Isso pode indicar:
  - Segmentos da empresa com menor engajamento;
  - Lideranças pouco eficazes;
  - Falta de comunicação ou reconhecimento em áreas específicas.
- **Atenção ao grupo insatisfeito:** Os **19,3% insatisfeitos** merecem análise especial — esse grupo pode ser o mais suscetível ao desligamento voluntário, absenteísmo ou baixo desempenho.
- **Base valiosa para cruzamentos:** Essa variável pode ser cruzada com:
  - **Turnover:** *quem sai mais: satisfeitos ou insatisfeitos?*;
  - **Horas Extras:** *trabalhadores mais sobrecarregados tendem a estar menos satisfeitos?*;
  - **Área/Cargo:** *quais setores têm mais colaboradores insatisfeitos?*.

##### Variável - ⚖️ Equilíbrio de Vida

<div align="center">
<img src= https://github.com/user-attachments/assets/a017e073-c5a4-42d0-b17f-5091765bc417
  alt="Satisfação com o Clima Organizacional" width="500" height="300">
  <p><strong> Figura 8:</strong> Satisfação com o Clima Organizacional.</p>
</div> 

🔑*Interpretações e reflexões:*
A variável Equilíbrio de Vida é uma peça-chave quando falamos de bem-estar, produtividade e retenção de talentos.
- Ambiente positivo para equilíbrio vida-trabalho: Cerca de **71% dos colaboradores** avaliam seu equilíbrio como **“Muito bom”** ou **“Excelente”**, o que é um ótimo sinal de cultura organizacional saudável.
- Baixo percentual de insatisfação grave: Apenas **5,4% reportam “Equilíbrio de vida ruim”**, sugerindo que a empresa pode estar gerenciando bem cargas de trabalho, horários e flexibilidade — ou que existem nichos específicos com esse desafio.
- Grupo intermediário relevante (**23,4% “Bom”**): Embora satisfeito, esse grupo pode sinalizar oportunidades de melhoria — são pessoas que talvez estejam no limite entre a satisfação e a sobrecarga.
- Base para cruzamentos estratégicos:
 Essa variável pode revelar muito quando combinada com:
  - Horas Extras: *quem tem baixo equilíbrio está fazendo mais horas?*
  - Satisfação no trabalho: *há coerência entre quem está satisfeito e quem sente equilíbrio?*
  - Turnover: *desequilíbrio está influenciando nas saídas?*

#### Análises Univariada. Variáveis Quantitativa Discreta

##### Variável - 🗓 Idade

Esta análise por faixas etárias, o que nos ajuda a entender melhor a distribuição demográfica da força de trabalho.

<div style="display: flex; justify-content: center; gap: 30px;">
  <div align="center">
    <img src="https://github.com/user-attachments/assets/2045dc76-a6a9-4041-9f76-6a8677533637" alt="Boxplot de Idade" width="400"/>
    <p><strong>Figura 9:</strong> Boxplot da Faixa Etária</p>
  </div>
  <div align="center">
    <img src="https://github.com/user-attachments/assets/4011794d-150e-456b-957e-85f773496f34" alt="Histograma de Idade" width="400"/>
    <p><strong>Figura 10:</strong> Histograma da Faixa Etária</p>
  </div>
</div>

Interpretação do Boxplot — Idade dos Colaboradores
🧮 Estatísticas Chave (extraídas do gráfico):
- **Mínimo:** 18 anos
- **Q1** (1º Quartil): 30 anos
- **Mediana:** ~36,92 anos
- **Q3** (3º Quartil): 43 anos
- **Máximo:** 60 anos
  
📌 O que esse *boxplot* revela:
- **Distribuição equilibrada:** A mediana está relativamente centralizada entre Q1 e Q3, indicando uma distribuição simétrica e saudável.
- **Amplitude interquartil (AIQ):** Compreendida entre 30 e 43 anos (13 anos), o que sugere uma **alta concentração de funcionários adultos jovens** — corroborando os dados por faixa etária que analisamos antes.
- **Sem outliers visíveis:** O gráfico não mostra pontos isolados além dos limites, sugerindo que **não há idades muito distantes do padrão**, como colaboradores extremamente jovens ou idosos.
- **Faixa etária bem distribuída entre 18 e 60 anos**, o que denota diversidade geracional dentro da empresa.

🔍 Complemento à análise do boxplot

- O histograma evidencia a forma da distribuição (quase normal, com leve inclinação à esquerda), enquanto o boxplot foca na mediana, dispersão e outliers.
- Ambos juntos mostram que **a idade média gira em torno de 36–37 anos**, sem extremos anômalos.

🔑*Interpretações e reflexões:*
- **Concentração nas faixas de 28 a 42 anos**: Juntas, as faixas **28–32 (16,96%)**, **33–37 (21,36%)** e **38–42 (17,86%)** representam mais da **metade da força de trabalho (56%)**. Isso sugere um time majoritariamente **adulto jovem a meia-idade**, faixa etária associada a maior produtividade, experiência consolidada e fase de estabilidade na carreira.
- **Baixa presença de jovens (18–27):** Apenas **9,3%** dos funcionários têm até 27 anos, o que pode indicar:
    - Baixa taxa de entrada de recém-formados ou estagiários;
    - Necessidade de revisar políticas de atração de jovens talentos.
- **Faixa sênior com representação modesta:** As faixas **53–57 (7,74%)** e **58–62 (3,14%)** somam cerca de **10,9%**. Esses profissionais podem representar papéis estratégicos ou lideranças seniores — importantes para retenção do conhecimento institucional.
- **Potencial para análise de rotatividade:** Ao cruzar com a variável “Deixou a Empresa”, poderemos identificar se **a rotatividade é mais comum entre os jovens (perfil exploratório)** ou os mais experientes (aposentadoria ou mudança de carreira).




---



##### Variável ***Target***: Funciónarios que deixaram a empresa
🔑Interpretações e reflexões:
- A taxa de turnover total de 16.1% no último ano:
   º Dos 1.470 funcionários analisados, **237 se desligaram da empresa**, representando **16,1% do total**. Esse índice está **abaixo da média nacional** e até de alguns benchmarks do setor de tecnologia[^1][^4], o que pode indicar **bons esforços atuais** em retenção — mas também **potencial para melhoria**

<p align="center">
<img src="https://github.com/user-attachments/assets/bacd97bc-af82-423e-b8e8-3b8a03fd2101" 
  alt="Descrição da imagem" width="400" height="300">
</p>

##### Variável: Funciónarios que deixaram a empresa
🎯Insights:

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

[^9]: TOWARDS DATA SCIENCE. *Using CRISP-DM to Grow as a Data Scientist*. Publicado em 2 abr. 2020. Disponível em: [https://towardsdatascience.com/using-crisp-dm-to-grow-as-data-scientist-a07ce3fd9d56](https://towardsdatascience.com/using-crisp-dm-to-grow-as-data-scientist-a07ce3fd9d56)

[^10]: ESTATÍSTICA FÁCIL. *O que é: Análise Exploratória de Dados*. Disponível em: [https://estatisticafacil.org/glossario/o-que-e-analise-exploratoria-de-dados/](https://estatisticafacil.org/glossario/o-que-e-analise-exploratoria-de-dados/)

 
