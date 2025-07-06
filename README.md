<p align="center">
  <img src="https://github.com/user-attachments/assets/1e0540ec-e599-4f33-8eda-886dbe2eeccf" alt="Imagem de portada">
</p>

# Projeto People Analytics: Redução do Turnover com CRISP-DM
 Projeto da formação "**Gerando Valor com Dados**" da Escola de Dados [Preditiva.IA](https://www.preditiva.ai.com)

## Índice
- [Contextualização](#Contextualização)
   - [Benchmark de Turnover no Setor de Tecnologia no Brasil.](#Benchmark-de-Turnover-no-Setor-de-Tecnologia-no-Brasil)
- [Metodologia CRISP DM](#Metodologia-CRISP-DM)
  - [Etapa 1: Compreensão do Negócio](#Etapa-1:-Compreensão-do-Negócio)
  - [Etapa 2: Compreensão dos Dados](#Etapa-2:-Compreensão-dos-Dados)
     - [Variáveis Qualitativas Nominal](#Variáveis-Qualitativas-Nominal)
     - [Variáveis Qualitativas Ordinal](#Variáveis-qualitativas-Ordinal)
     - [Variáveis Quantitativa Discreta](#Variáveis-Quantitativa-Discreta)
     - [Variáveis Quantitativa Contínua](#Variáveis-Quantitativa-Continua)
     - [Matriz Geral. Perfil de Todos os Funcionários](#Matriz-Geral—.Perfil-de-Todos-os-Funcionários)
     - [Perfil Padrão de Funcionário com Alta Propensão ao Turnover](#Perfil-Padrão-de-Funcionário-com-Alta-Propensão-ao-Turnover)
   - [Etapa 3: Preparação dos Dados](#Etapa-3-Preparação-dos-Dados)
   - [Etapa 4: Modelagem ou Análises](#Etapa-4-Modelagem-ou-Análises)
   - [Etapa 5: Avaliação](#Etapa-5-Avaliação)
      - [Interpretação dos resultados obtidos apartir do cálculo do IV](#Interpretação-dos-resultados-obtidos-apartir-do-cálculo-do-iv)
      - [Comparação com benchmarks do setor para validar insights](#Comparação-com-benchmarks-do-setor-para-validar-insights)
   - [Etapa 6 Implantação](#Etapa-6-Implantação)
      - [Plano de Ação: Redução de Turnover com base em variáveis críticas](#Plano-de-Ação:–Redução-de-Turnover-com-base-em-variáveis-críticas)
      - [Métricas para Acompanhamento da Retenção de Funcionários](#Métricas-para-Acompanhamento-da-Retenção-de-Funcionários)
 - [Referências](#Referências)

##  Contextualização  

### O desafio do ***turnover*** nas empresas  

O ***turnover*** ou **rotatividadedos funcionários**, é um dos desafios mais críticos enfrentados pelas empresas atualmente. Segundo um levantamento publicado em **agosto de 2023** pela consultoria **Robert Half**, o Brasil lideravá o ranking global de rotatividade nesse ano, com uma taxa de **56%**, colocando o país entre os que mais enfrentam desafios com retenção de talentos. Esse índice elevado reflete mudanças estruturais no mercado de trabalho, impulsionadas por transformações nas expectativas dos profissionais, que estão cada vez mais atentos ao propósito, à flexibilidade e ao equilíbrio entre vida pessoal e profissional [^1].

Outro estudo publicado pela **Evermonte** em **julho de 2024** apontou que **39% dos desligamentos no Brasil em 2023 foram voluntários**, ou seja, motivados pela decisão dos próprios colaboradores[^2]. Esse dado reforça que fatores como satisfação profissional, oportunidades de crescimento e ambiente organizacional exercem influência direta na retenção de talentos, evidenciando a necessidade de estratégias mais humanas e personalizadas por parte das empresas.

### Benchmark de ***Turnover*** no Setor de Tecnologia no Brasil  
Para contextualizar melhor este projeto, é essencial entender a taxa de rotatividade no setor de tecnologia e como a empresa analisada se compara ao mercado. 


###  Visão Geral  

- A média de rotatividade no Brasil -área de tecnología-  ficou em **51%** entre abril de 2022 e maio de 2023, uma das mais altas do mundo[^3] 
- No setor de tecnologia, a taxa média de turnover foi de **13,2%**, a maior entre todos os setores avaliados[^4].  
- Em comparação global, é comum observar taxas entre **13% e 18% ao ano** no setor de tecnologia, podendo chegar a **25%** em startups[^5].  

###  Comparações e Dados Históricos  

° Antes da pandemia (2019), o turnover médio no setor de TI no Brasil era de **39%**, enquanto a média geral era **41%**[^6].  
° Subsetores como desenvolvimento de software apresentavam taxas menores (**33%–39%**)[^6].  
° Cargos executivos de tecnologia no Brasil apresentam turnover voluntário de **20%** e involuntário de **14%**, totalizando **34%**[^7].  

###  Segmentação por Subárea  

- **UX e Design**: aproximadamente **23%** [^8];  
- **Engenheiros de Dados e Software**: entre **21% e 22%** [^8]; 
- **Suporte técnico e áreas de operação**: **até 25%**[^8]. 

### Insight para o Projeto  

Com base nesses dados, uma meta realista para a organização é redução da taxa de turnover **abaixo de 15%**, posicionando-se entre os **benchmarks** mais estáveis do setor de tecnologia nacional e internacional e determinar quais políticas/fatores deveriam mudar de forma a minmizar o turnover

### Estratégias para minimizar o turnover  

Diante desse cenário, e com base às pesquesisas abordadas anteriormente, foram identificados estratégicas inovadores que as empresas precisam adotar para reduzir a rotatividade. Algumas abordagens incluem:  

- **Criar um ambiente de trabalho dinâmico**, onde os funcionários sintam que estão evoluindo constantemente.  
- **Investir em aprendizado contínuo**, incentivando o desenvolvimento profissional.  
- **Ouvir os colaboradores**, garantindo que suas necessidades e expectativas sejam atendidas.  

O ***turnover*** não é apenas uma questão de remuneração, mas sim de **propósito e engajamento**. Empresas que conseguem oferecer um ambiente estimulante e oportunidades de crescimento tendem a reter seus talentos por mais tempo.  

## Metodologia - CRISP-DM

###  O que é CRISP-DM?  

A metodologia ***CRISP-DM (Cross Industry Standard Process for Data Mining)*** é um modelo padrão amplamente utilizado para projetos de **Data Science** e **Machine Learning**. Criada nos anos 1990, essa abordagem orienta o processo de análise de dados em **seis fases estruturadas**, garantindo que cada etapa seja bem definida e alinhada aos objetivos do negócio.  

###  Por que utilizar CRISP-DM neste projeto?  

Este projeto busca **entender os fatores que influenciam o turnover** e propor **estratégias para reduzir a rotatividade** dos funcionários em uma empresa de tecnologia. Como se trata de uma análise exploratória e investigativa, a CRISP-DM é a metodologia ideal, pois oferece um fluxo de trabalho lógico e sistemático para abordar o problema de forma eficiente.  

<div align="center">
  <img src="https://github.com/user-attachments/assets/c5129457-0470-44cb-b0b2-cadf5b2de4fd" alt="Box plot dos salários" width="500" height="500"/>
  <p><strong>Figura 1:</strong> Modelo de processo CRISP-DM</p>
  <p style="font-size: 0.9em;">
    <em>Fonte:</em> TOWARDS DATA SCIENCE. <strong>Using CRISP-DM to Grow as a Data Scientist</strong>. Publicado em 2 abr. 2020.
    Disponível em: <a href="https://towardsdatascience.com/using-crisp-dm-to-grow-as-data-scientist-a07ce3fd9d56" target="_blank">https://towardsdatascience.com/...</a>
  </p>
</div>

###  As seis fases do CRISP-DM e sua aplicação no projeto  

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

### Benefícios da CRISP-DM para este estudo  

 **Estruturação clara do processo de análise**  
 **Maior confiabilidade nos resultados obtidos**  
 **Facilidade na comunicação dos insights ao RH e gestores**  
 **Melhor alinhamento entre dados e tomada de decisão**  

Com essa metodologia, garantimos que o projeto será conduzido de forma **organizada, eficiente e baseada em evidências**, trazendo insights valiosos para reduzir o turnover na empresa de tecnologia.  

## Metodologia - CRISP-DM. Framework de Análise de Dados. 

### Etapa 1: Compreensão do Negócio (Business Understanding)

Para compreender quais são as características que fazem um funcionário ficar ou deixar a empresa de Tecnologia, o departamento de Recursos Humanos da empresa catalogou informações de **1.470 funcionários** que 
deixaram ou permaneceram na companhia no *último ano*. O resultado desse levantamento gerou **19 possíveis fatores** para tentar explicar o comportamento do ***turnover***. Para conhecer esses fatores, verifique a tabela de metadados
existentes na secção seguinte ou na pasta */docs/* no arquivo .xlsx *classificação_variaveis_turnover*

####  Objetivo do projeto:
- **Reduzir** o ***turnover*** e **melhorar a retenção dos funcionários** meio da análise de dados comportamentais, profissionais e demográficos dos colaboradores.
- **Identificar** quais **fatores** mais influenciam a saída dos colaboradores.
- **Criar um plano de ação** *5W2H* baseado nos insights obtidos, propondo estratégias para minimizar a rotatividade.

####  Impacto do turnover:
- Custos elevados com recrutamento e treinamento.
- Perda de produtividade e conhecimento institucional.
- Impacto na cultura e no clima organizacional.

####  Variáveis que podem explicar o turnover:
- Dados demográficos (*idade, gênero, estado civil*).
- Características do trabalho (*salário, equilíbrio entre vida pessoal e profissional*).
- Ambiente corporativo (*satisfação organizacional, relação com o chefe*).
- Histórico do funcionário (*tempo de empresa, promoção, mudanças de cargo*).
  
####  Perguntas estratégicas para investigação:
- *Quais políticas/fatores da empresa deveriam mudar de forma a minimizar o turnover*
- *O turnover é maior em algum grupo específico de funcionários?*
- *Existe correlação entre salário, tempo de empresa e saída voluntária?*
- *Como o clima organizacional impacta a retenção dos talentos?*
- *Funcionários que viajam frequentemente são mais propensos a sair?*

---

###  Etapa 2: Compreensão dos Dados (Data Understanding)

Após a definição clara do problema de negócio e dos objetivos estratégicos do projeto, o próximo passo consiste em explorar a base de dados fornecida pelo departamento de Recursos Humanos. Para isso, foi disponibilizado um arquivo no formato **.xlsx**, contendo informações de **1.470 funcionários** que permaneceram ou deixaram a empresa no último ano. A base contempla variáveis de diferentes naturezas — **demográficas, funcionais e comportamentais** — que foram organizadas e documentadas na tabela de **metadados**, facilitando a identificação e classificação de cada atributo. Ao todo, foram listadas **19 variáveis potencialmente associadas ao turnover**, como idade, salário, tempo na empresa, frequência de viagens, satisfação organizacional, entre outros fatores. 

O objetivo para esta etapa é **a compreensão de cada variavel, sua distribuição, e a identificação de variáveis relevantes com o ***turnover*** e a detecção de outliers**. Para ello, faremos uso da **Análise Exploratória de Dados (AED)** [^10] como abordagem fundamental na ciência e análesis de dados por meio da ferramenta *Microsoft® Excel®*. Além disso, durante esta etapa, e antes do *AED*, é crucial verificar a qualidade dos dados, por meio do chamado *Sanity Check*, permitindo identificar valores fora de faixas plausíveis -*outliers*-, anomalias ou registros possivelmente inconsistentes. 

###  Principais Técnicas Utilizadas nesta Etapa

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

Essas análises oferecem a base necessária para a próxima etapa do projeto — a preparação dos dados e construção de modelos que ajudem a identificar os fatores mais relevantes associados ao turnover.

####  Dicionário de Dados

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

####  Variável Alvo

- `Funcionário_deixou_a_empresa` — Indica se o funcionário deixou a empresa recentemente (`1`) ou não (`0`).

#### Análises Univariada. Variáveis Qualitativas Nominal

##### Variável - Gênero do funcionário

<div align="center">
<img src= https://github.com/user-attachments/assets/0efbeb3c-8aaa-4f26-ae66-d3d223308ee5
  alt="Fig. Distribuição de gênero dos funcionário entrevistados" width="400" height="370">
  <p><strong> Figura 2:</strong> Distribuição dos funcionários da empresa por genero: M(Mulheres) e H(Homens)</p>
</div> 

**Interpretações e reflexões:**
- **Distribuição equilibrada (mas levemente concentrada)**:
A equipe é composta por **60% de homens e 40% de mulheres**, o que mostra um certo equilíbrio, especialmente em comparação com a média de representatividade feminina no setor de tecnologia, que tende a ser mais baixa.
- **Ponto de atenção para a diversidade**:
Embora não haja um desequilíbrio alarmante, essa divisão pode servir como referência para **metas de inclusão e diversidade de gênero** dentro da organização, especialmente se refletir também em cargos de liderança e acesso a promoções.
- **Base para análises comparativas**:
Esse recorte será útil para verificar se há **diferenças significativas de turnover entre os gêneros**. Por exemplo:
- *A proporção de mulheres que se desligaram foi superior à de homens?*
- *O tempo médio de permanência é diferente entre os gêneros?* Infelizmente, esta questão não tem como ser abordada com as informações fornecidas pela empresa, porém, seria de suma importância contar com esses datos para futuras análises sobre o índice de *turnover* 
- Potencial para cruzamento com salário ou promoção:
Vale cruzar esse dado com outras variáveis como faixa salarial, número de promoções e satisfação no trabalho — é possível detectar, por exemplo, se há disparidades de gênero na remuneração ou reconhecimento.

##### Variável - Estado Civil

<div align="center">
<img src= https://github.com/user-attachments/assets/812bb551-af78-4db4-908c-9a99a9ff5110
  alt="Fig. Distribuição dos funcionários por Estado Civil" width="500" height="300">
  <p><strong> Figura 3:</strong> Distribuição dos funcionários por Estado Civil.</p>
</div> 

**Interpretações e reflexões:**
- **Predomínio de funcionários casados**: A maior parte da força de trabalho é casada (**45,8%**), o que pode indicar maior estabilidade, mas também maior responsabilidade financeira, familiar e demanda por equilíbrio vida-trabalho.
- **Perfil jovem-adulto em destaque:** A soma de **solteiros (32%) + divorciados (22,2%)** representa mais de **54% da amostra**, o que sugere um público majoritariamente com perfil de transição de carreira, mobilidade geográfica ou em busca de desenvolvimento profissional acelerado.
- Possível relação com o turnover: Funcionários solteiros ou divorciados, por estarem em fases de maior flexibilidade pessoal, podem apresentar maior propensão à rotatividade. Isso será especialmente importante ao cruzar com a variável “Deixou a empresa”.
- Atenção para políticas personalizadas: Esses dados servem como base para refletir sobre programas de retenção mais segmentados. Por exemplo, casados podem valorizar benefícios familiares ou flexibilidade de horários, enquanto solteiros podem se interessar mais por trilhas de crescimento e mobilidade interna

##### Variável - Funcionário costuma fazer horas extras? Sim/Não

<div align="center">
<img src= https://github.com/user-attachments/assets/aa4a3c12-76b5-491c-8d62-63ae257f3178
  alt="Fig.4 Proporção de Funcionários que Realizam Horas Extras" width="400" height="370">
  <p><strong> Figura 4:</strong> Proporção de Funcionários que Realizam Horas Extras.</p>
</div> 

*Interpretações e reflexões:*
- **A maioria dos colaboradores (71,7%) não realiza horas extras**, o que pode indicar um bom controle da carga de trabalho ou políticas eficazes de equilíbrio.
- **Quase 1 em cada 3 colaboradores faz horas extras (28,3%)** — esse grupo merece atenção especial, pois horas extras frequentes podem estar relacionadas a:
  - Sobrecarga de demandas em determinadas áreas;
  - Dificuldades de dimensionamento da equipe;
  - Potenciais gatilhos para rotatividade, principalmente se o esforço não estiver sendo compensado financeiramente ou reconhecido institucionalmente.
- Próximo passo interessante: Cruzar essa variável com: 
  - Turnover: Quem faz horas extras tem maior taxa de saída?
  - Satisfação no trabalho: Há correlação negativa?
  - Cargo ou área de atuação: As horas extras estão concentradas em setores específicos
    
##### Variável ***Target***: Funciónarios que deixaram a empresa
A variável-alvo (ou target) na análise de turnover, pois representa o comportamento que estamos tentando compreender e, se possível, prever.

<p align="center">
<img src= https://github.com/user-attachments/assets/d32b5fbe-8f07-4b6d-810a-2178e5761b71
 alt="Descrição da imagem" width="500" height="300">
</p>

Interpretações e reflexões:
- Turnover total de 16,1%:
Dos 1.470 funcionários analisados, **237 se desligaram da empresa**, representando **16,1% do total**. Esse índice está **abaixo da média nacional** e até de alguns benchmarks do setor de tecnologia[^1][^4], o que pode indicar **bons esforços atuais em retenção** — mas também potencial para melhoria.
- **Desequilíbrio entre as classes (classe desbalanceada)**:
O dado mostra que a maioria dos funcionários **permaneceu na empresa (83,9%)**, o que sugere que o conjunto está **desbalanceado**. Esse é um ponto crítico especialmente se futuramente for construída uma classificação preditiva, já que modelos podem tender a “aprender” mais sobre a classe majoritária e ignorar os desligamentos. Técnicas como oversampling ou stratified split serão importantes.
- Base de comparação para as demais análises:
Agora que temos a proporção entre quem saiu e quem ficou, podemos usá-la para:
  - Avaliar se determinadas faixas etárias, salários, cargos ou departamentos têm uma proporção de saída maior do que os 16,1% globais;
  - Realizar testes estatísticos (ex: testes de proporção ou chi-quadrado) para saber se essas diferenças são significativas;
  - Identificar fatores de risco mais relevantes para o desligamento


#### Análises Univariada. Variáveis Qualitativas Ordinal
##### Variável - Frequência de Viagens

<div align="center">
<img src= https://github.com/user-attachments/assets/f740c772-e045-4e52-8f1f-0bd7082d6109
  alt="Fig. Frequência de Viagens" width="500" height="400">
  <p><strong> Figura 5:</strong> Distribuição de Funcionários por Frequência de Viagens.</p>
</div> 


*Interpretações e reflexões:*
- A maior parte dos colaboradores (**71%**) viaja raramente, sugerindo que a empresa adota um modelo com deslocamentos pontuais, talvez mais comum em funções técnicas ou administrativas.
- Quase 19% viaja com frequência, o que pode indicar funções voltadas à área comercial, suporte externo ou cargos executivos — esses colaboradores podem estar mais expostos a fatores de estresse, desequilíbrio vida-trabalho e potencial desgaste, especialmente se não houver compensações compatíveis.
- Apenas **10,2%** não viajam nunca, o que pode incluir funções exclusivamente internas, como suporte local, administrativo, ou posições mais júnior.

##### Variável - Formação Acadêmica
<div align="center">
<img src= https://github.com/user-attachments/assets/5d48e22e-5712-481b-a3bd-39164a9f6d63
  alt="Fig. Formação Acadêmica" width="500" height="300">
  <p><strong> Figura 6:</strong> Distribuição de Funcionários por Nível de Formação Acadêmica.</p>
</div> 

*Interpretações e reflexões:*

- **Alta escolaridade da força de trabalho:** Cerca de **69% dos colaboradores possuem Ensino Superior ou Pós-Graduação (Mestrado/Doutorado)**. Isso sugere que a empresa opera em um contexto técnico ou altamente qualificado — possivelmente setores como tecnologia, pesquisa, engenharia ou serviços especializados.
- **Pico em Ensino Superior:** A maior parte está concentrada no Ensino Superior **(38,9%)**, seguido de Mestrado **(27,1%)**, o que indica **forte cultura de qualificação acadêmica** e uma provável valorização de títulos na progressão de carreira.
- **Baixa presença de Ensino Médio:** Apenas **11,6%** têm formação média, o que pode representar cargos operacionais ou de apoio com menor exigência técnica. Isso pode impactar o perfil de turnover nesses grupos (por exemplo: maior rotatividade por remuneração ou oportunidades externas).
- Doutorado é minoria, mas relevante: Com 48 pessoas **(3,3%)**, essa faixa pode representar áreas de inovação, pesquisa ou liderança técnica. Esses profissionais tendem a ter expectativas mais elevadas de desafios, autonomia e reconhecimento.

Potencial de Cruzamentos
Essa variável pode ser extremamente reveladora quando cruzada com:
- Salário Mensal: *Há proporcionalidade entre formação e remuneração?*
- Turnover: *Profissionais com maior formação estão deixando a empresa mais ou menos?*
- Promoção / Crescimento na empresa: *Qual o impacto da formação na trajetória interna?*

##### Variável - Satisfação com o Clima Organizacional

<div align="center">
<img src= https://github.com/user-attachments/assets/4f2f0353-549b-42e9-891e-d7d01ba84e3d
   alt="Satisfação com o Clima Organizacional" width="500" height="400">
  <p><strong> Figura 7:</strong> Satisfação com o Clima Organizacional.</p>
</div> 

*Interpretações e reflexões:*
Esta variável é altamente relevante para prever engajamento, produtividade e riscos de desligamento.
- **Clima amplamente positivo:** Quase **61% dos colaboradores** relataram níveis de satisfação **"Alto"** ou **"Muito Alto"**. Isso demonstra um ambiente organizacional saudável e colaborativo — uma excelente base para retenção e desempenho.
- **Dois polos bem definidos:** Enquanto boa parte demonstra alta satisfação, há um bloco expressivo de colaboradores (**38,8%**) com níveis **"Baixo"** ou **"Médio"**. Isso pode indicar:
  - Segmentos da empresa com menor engajamento;
  - Lideranças pouco eficazes;
  - Falta de comunicação ou reconhecimento em áreas específicas.
- **Atenção ao grupo insatisfeito:** Os **19,3% insatisfeitos** merecem análise especial — esse grupo pode ser o mais suscetível ao desligamento voluntário, absenteísmo ou baixo desempenho.


##### Variável -  Equilíbrio de Vida

<div align="center">
<img src= https://github.com/user-attachments/assets/5c19c18b-4e1f-4941-a7cc-d49ca9868f81
  alt="Satisfação com o Clima Organizacional" width="500" height="300">
  <p><strong> Figura 8:</strong> Satisfação com o Clima Organizacional.</p>
</div> 

*Interpretações e reflexões:*
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

##### Variável - Idade

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
 Estatísticas Chave (extraídas do gráfico):
- **Mínimo:** 18 anos
- **Q1** (1º Quartil): 30 anos
- **Mediana**: 36 anos
- **Média:** ~36,92 anos
- **Q3** (3º Quartil): 43 anos
- **Máximo:** 60 anos
  
 O que esse *boxplot* revela:
- **Distribuição equilibrada:** A mediana está relativamente centralizada entre Q1 e Q3, indicando uma distribuição simétrica e saudável.
- **Amplitude interquartil (AIQ):** Compreendida entre 30 e 43 anos (13 anos), o que sugere uma **alta concentração de funcionários adultos jovens** — corroborando os dados por faixa etária que analisamos antes.
- **Sem outliers visíveis:** O gráfico não mostra pontos isolados além dos limites, sugerindo que **não há idades muito distantes do padrão**, como colaboradores extremamente jovens ou idosos.
- **Faixa etária bem distribuída entre 18 e 60 anos**, o que denota diversidade geracional dentro da empresa.

 Complemento à análise do boxplot

- O histograma evidencia a forma da distribuição (quase normal, com leve inclinação à esquerda), enquanto o boxplot foca na mediana, dispersão e outliers.
- Ambos juntos mostram que **a idade média gira em torno de 36–37 anos**, sem extremos anômalos.

*Interpretações e reflexões:*
- **Concentração nas faixas de 28 a 42 anos**: Juntas, as faixas **28–32 (16,96%)**, **33–37 (21,36%)** e **38–42 (17,86%)** representam mais da **metade da força de trabalho (56%)**. Isso sugere um time majoritariamente **adulto jovem a meia-idade**, faixa etária associada a maior produtividade, experiência consolidada e fase de estabilidade na carreira.
- **Baixa presença de jovens (18–27):** Apenas **9,3%** dos funcionários têm até 27 anos, o que pode indicar:
    - Baixa taxa de entrada de recém-formados ou estagiários;
    - Necessidade de revisar políticas de atração de jovens talentos.
- **Faixa sênior com representação modesta:** As faixas **53–57 (7,74%)** e **58–62 (3,14%)** somam cerca de **10,9%**. Esses profissionais podem representar papéis estratégicos ou lideranças seniores — importantes para retenção do conhecimento institucional.
- **Potencial para análise de rotatividade:** Ao cruzar com a variável “Deixou a Empresa”, poderemos identificar se **a rotatividade é mais comum entre os jovens (perfil exploratório)** ou os mais experientes (aposentadoria ou mudança de carreira).

##### Variável - Distância do Trabalho

A variável Distância do Trabalho nos oferece um ótimo panorama sobre mobilidade, logística e até possíveis influências no bem-estar e na rotatividade dos colaboradores

<div align="center">
<img src= https://github.com/user-attachments/assets/425ff717-b052-4243-b001-250939529b52
  alt="Distância do Trabalho" width="500" height="300">
  <p><strong> Figura 11:</strong> Boxplot distância do trabalho dos colaboradores.</p>
</div> 

Interpretação do Boxplot
 Elementos estatísticos do gráfico:
- **Mínimo**: 1 km
- **1º quartil** (Q1): 2 km
- **Mediana**: 7 KM
- **Média**: 9,19 km
- **3º quartil** (Q3): 14 km
- **Máximo**: 29 km

 O que esse *boxplot* revela:
- **Distribuição assimétrica à direita (assimetria positiva)**:
A maior parte dos colaboradores reside próximo ao trabalho, com valores concentrados entre **1 e 14 km** -*~75% dos funcionários*-, mas há uma **cauda estendida até 29 km**, indicando alguns casos de deslocamentos mais longos.
- **Mediana deslocada para a esquerda da caixa:**
A mediana está mais próxima do Q1 do que do Q3, o que confirma que *mais de 50% dos funcionários vivem a menos de 7 km da empresa*. Excelente indicador logístico!
- **Ausência de outliers visíveis:**
Não há pontos fora do intervalo da caixa com bigodes, o que indica que **os deslocamentos estão bem distribuídos e dentro de uma faixa aceitável**.
- **Amplitude interquartil (IQR):**
A faixa central da maioria dos funcionários está entre **2 km e 14 km**, o que ajuda a delimitar uma zona de "conforto logístico" para políticas de home office parcial ou benefícios de mobilidade.

*Interpretações e reflexões:*
- **Alta concentração próxima ao local de trabalho:**
Mais de **1/3 dos colaboradores (34,2%) moram até 3 km da empresa**, o que pode sugerir:
  - Boa localização da empresa;
  - Preferência por contratação local;
  - Menores custos de transporte e maior pontualidade.
- **Distribuição decrescente com a distância:**
À medida que a distância aumenta, o número de funcionários diminui — mostrando que a empresa **atrai menos pessoas de áreas mais distantes**, o que é esperado.
- **Grupo entre 7 e 12 km (26% combinados)** ainda representa uma parcela relevante, possivelmente motivada por facilidade de transporte público ou compensações oferecidas.
- **Maioria mora até 9 km da empresa (63,9%)**, o que confirma um padrão de deslocamento moderado e confortável para boa parte da força de trabalho.
- **Distâncias acima de 18 km (faixas finais)** somam apenas cerca de **17% do total**, mas esse grupo pode ter:
  - Desgaste com o deslocamento;
  - Demanda por modelos híbridos ou flexíveis.

##### Variável -  Quantidade de Empresas que um Funcionário Trabalhou

 A variável "Quantidade de Empresas que um Funcionário Trabalhou" é uma excelente proxy para entender experiência prévia, perfil profissional e até possível propensão ao turnover. Vamos destrinchar os insights:

<div align="center">
<img src= https://github.com/user-attachments/assets/7b24819f-ea03-4e1e-8265-9498e32a8f99
  alt="Satisfação com o Clima Organizacional" width="500" height="300">
  <p><strong> Figura 12:</strong> Boxplot quantidade de empresas que um funcionário trabalhou.</p>
</div> 

Interpretação do Boxplot:
 Estatísticas visuais extraídas do gráfico:
- **Mínimo**: 0 empresas
- **Q1** (1º quartil): 1 empresa
- **Mediana** (Q2): 2 empresas
- **Média**: cerca de 2,7 empresas
- **Q3** (3º quartil): 4 empresas
- **Máximo**: 9 empresas
- **Outlier identificado**: 9 empresas (isolado acima dos bigodes

 Interpretações:
- **Distribuição assimétrica à direita (positivamente enviesada)**:
A mediana está mais próxima de Q1 que de Q3, e o boxplot apresenta uma cauda longa à direita, indicando que a **maioria dos funcionários trabalhou em até 4 empresas**, mas há alguns com trajetórias mais instáveis ou extensas.
- **Concentração de históricos curtos**:
Com Q1 em 1 e mediana em 2, isso reforça que **pelo menos 50% dos colaboradores têm uma experiência profissional mais enxuta**, o que pode indicar:
    - Profissionais em início de carreira;
    - Menor bagagem de mercado (mas talvez maior lealdade organizacional).
- **Outlier interessante**:
O valor **9 como ponto extremo isolado** pode representar perfis com alta mobilidade — seja por desejo de crescimento rápido, instabilidade de carreira, ou funções temporárias.

*Interpretações e reflexões:*
- **Quase metade dos funcionários (48,8%) trabalharam em no máximo uma empresa antes da atual** — ou seja, **são profissionais com pouca experiência anterior ou que iniciaram a carreira na empresa atual**. Esse grupo tende a apresentar:
    - Menor exposição a outras culturas organizacionais;
    - Possivelmente mais lealdade ou dependência da empresa atual;
    - Alto potencial para retenção, *se houver investimento em desenvolvimento.*
- **51,2% já passaram por 2 ou mais empresas**, o que pode indicar:
    - Profissionais **com bagagem de mercado** e diversidade de experiências;
    - Perfil mais exploratório ou ambições de crescimento acelerado — o que pode estar correlacionado a uma **maior tendência à rotatividade**.
- **Grupo com 6 a 9 empresas (16,7%)**: Possível sinal de mobilidade elevada ou até um histórico de trocas frequentes. Vale analisar:
    - Se esse grupo permanece menos tempo na empresa atual;
    - Como se comportam em termos de satisfação e equilíbrio.

##### Variável - Quantidade de Ações da Empresa
 A variável Quantidade de Ações da Empresa revela muito sobre o grau de engajamento, a credibilidade, confiança e participação dos colaboradores no negócio

<div align="center">
<img src= https://github.com/user-attachments/assets/4f1c94f1-8fe1-41aa-920d-f2a8a5d7112f
  alt="Variável Quantidade de Ações da Empresa" width="500" height="300">
  <p><strong> Figura 13:</strong> Gráfico Quantidade de Ações da Empresa que possuem os funcionários.</p>
</div> 

*Interpretações e reflexões:*
- **Cerca de 43% dos colaboradores não possuem ações da empresa**, o que pode indicar:
    - Falta de interesse ou entendimento sobre o programa de participação acionária;
    - Elegibilidade restrita ou falta de incentivo para adesão;
    - Perfil de colaboradores mais novos, operacionais ou menos engajados com a cultura corporativa.
- **41% possuem 1 ação**, o que mostra um nível básico de envolvimento — pode indicar que esses colaboradores participaram de iniciativas pontuais ou receberam ações em programas padronizados.
- **Somente 16,5% possuem 2 ou mais ações**, sugerindo um grupo mais envolvido, veterano ou que aposta na empresa como plano de longo prazo — esses funcionários tendem a ter **maior alinhamento com os resultados organizacionais**, e possivelmente ocupam **posições de liderança, cargos técnicos estratégicos ou estão na empresa há mais tempo**.
- **Distribuição decrescente** reforça a ideia de que a posse de ações está fortemente concentrada em um grupo pequeno e mais engajado.

##### Variável - Tempo de Carreira (em anos)
Excelente variável para entender a maturidade profissional da equipe, analisaro o **Tempo de Carreira em anos**, que é uma proxypodereso para avaliar asenioridade, estabilidade e potencial de desenvolvimento interno.

<div style="display: flex; justify-content: center; gap: 30px;">
  <div align="center">
    <img src="https://github.com/user-attachments/assets/d2c6e220-5c76-4b27-8f44-f1de33ce81c3" width="400"/>
    <p><strong>Figura 14:</strong> Boxplot Tempo de Carreira em anos</p>
  </div>
  <div align="center">
    <img src="https://github.com/user-attachments/assets/b6fa15a7-77f1-48b0-adb4-b8d3cce644bc" alt="Histograma de Tempo de Carreira em anos" width="400"/>
    <p><strong>Figura 15:</strong> Histograma do Tempo de Carreira em anos</p>
  </div>
</div>

*Interpretações e reflexões:*

 TABELA *de frequência*
- A maior parte dos colaboradores (73%) tem até **14 anos de carreira**, com pico na faixa de **5–9 anos (33,5%)**.
- As faixas mais experientes (25+ anos) são minoria: apenas **~7% do total**.
- A distribuição sugere uma equipe majoritariamente em **fase de consolidação de carreira** (nem muito nova, nem perto da aposentadoria).

Boxplot
- **Mediana**: 10 anos
- **Média**: 11,28 anos (ou seja, > mediana → assimetria à direita)
- **Quartis**: Q1 ≈ 6 anos e Q3 ≈ 15 anos
- **Outliers**: valores acima de 30 anos (30, 33, 37, 40) indicam perfis muito seniores.
   O boxplot confirma:
- Que a maioria está entre 6 e 15 anos de carreira;
- Que existem **alguns poucos casos muito acima da média** (outliers), puxando a média para cima.

 Histograma
- A cauda direita é longa (mais valores extremos positivos), o que reforça a distribuição assimétrica à direita.
- O maior pico (classe modal) está na faixa de **5–9 anos**, seguido pela faixa **0–4**.
- Frequência decrescente conforme o tempo de carreira aumenta.
- O histograma dá uma visão visual da **frequência por classe**, mostrando onde está a maior massa da população e reforçando a leitura do boxplot.

Conclusão Integrada

>A distribuição do tempo de carreira da equipe é **concentrada em profissionais com até 15 anos de experiência**, com média em torno de 11 anos e uma **leve assimetria positiva**. Isso indica uma equipe **jovem-madura**, com forte potencial de crescimento, aprendizado e retenção. Os poucos colaboradores com mais de 30 anos de carreira são outliers valiosos, provavelmente ocupando funções de liderança, mentoria ou expertise técnica.

##### Variável - Horas de Treinamento

<div align="center">
<img src= https://github.com/user-attachments/assets/80d97542-3c68-4d98-887f-e953b9cd600c
  alt="Horas de Treinamento" width="500" height="300">
  <p><strong> Figura 16:</strong> Boxplot Horas de Treinamento dos funcionários.</p>
</div> 

*Interpretações e reflexões:*
- A grande maioria dos colaboradores realizou **2 ou 3 horas de treinamento** — cerca de **70,6% da amostra**.
- Apenas **3,7% não participaram de nenhum treinamento**, enquanto menos de **9% fizeram mais de 5 horas**.
- Isso indica uma política de capacitação concentrada em **ações curtas e padronizadas**.

Interpretação do Boxplot:
- **Mínimo**: 0 horas
- **Q1 (25%)**: 1 hora
- **Mediana**: 2,5 horas
- **Média**: 2,8 horas
- **Q3 (75%)**: 3 horas
- **Máximo (sem outlier)**: 4 horas
- **Outliers identificados**: 5 e 6 horas (valores superiores isolados)

   Insights do Boxplot:
- **Distribuição assimétrica à direita**: maioria dos colaboradores está concentrada entre 2 e 3 horas, com poucos realizando 5–6 horas (outliers).
- **Média > mediana** (média próxima de 2,8): confirma a assimetria positiva — algumas pessoas fizeram mais horas e puxaram a média para cima.
- **Amplitude interquartil (IQR)**: de 1 a 3 horas — ou seja, 50% da equipe recebeu um treinamento bastante breve.

 Conclusão Integrada
>A análise mostra que **a política de treinamento da empresa é fortemente concentrada em ações curtas e padronizadas**, com dois terços dos funcionários recebendo de 2 a 3 horas de capacitação. O boxplot destaca **uma leve assimetria à direita**, puxada por colaboradores que receberam 5 ou 6 horas — possivelmente líderes, áreas técnicas ou grupos-alvo específicos. A baixa presença de valores extremos também sinaliza uniformidade no modelo de treinamento adotado.

##### Variável - Tempo de Empresa (em Anos)

Com a análises desta variváel conseguimos ter uma leitura muito rica da permanência dos funcionários ao logo dos anos.

Análises da Composição da Tabela de frequência:

- Mais de 52% dos colaboradores têm até 5 anos de casa — alta proporção de profissionais “jovens” na organização.
- Apenas 4,5% têm mais de 20 anos de casa, mostrando uma base sênior pequena.

<div align="center">
<img src= https://github.com/user-attachments/assets/d1a73e53-e1e9-4b79-bfab-fb7c967ccb8d
  alt="Horas de Treinamento" width="500" height="300">
  <p><strong> Figura 17:</strong> Boxplot Tempo de Empresa - em anos - dos colaboradores.</p>
</div> 

Análise do Boxplot
- **Mínimo**: 0 anos
- **Q1**: ~3 anos
- **Mediana**: 5 anos
- **Média**: 7,01 anos
- **Q3**: ~9 anos
- **Máximo** (sem outliers): 18 anos
- **Outliers identificados**: de 19 a 40 anos de empresa
  
A cauda longa para a direita indica assimetria positiva, com poucos profissionais que ficaram décadas e puxam a média para cima.
O corpo da caixa entre 3 e 9 anos reforça que a maioria está estabilizada, mas ainda em fase de meia permanência.

Tabela 2: Integração entre Boxplot e Tabela
| Perspectiva              | Tabela                          | Boxplot                                 |
|--------------------------|---------------------------------|------------------------------------------|
| Colaboradores novatos    | 23,3% até 2 anos                | Início do bigode inferior                |
| Coração da distribuição  | 3–9 anos = 46,2%                | Entre Q1 e Q3                            |
| Alta permanência (senior)| <10% com 15+ anos               | Outliers extremos identificados          |


*Interpretações e reflexões:*
- A empresa tem uma composição predominantemente **júnior a intermediária em tempo de casa** — o que é comum em organizações em crescimento ou com rotatividade natural moderada.
- A mediana em 5 anos mostra que, apesar da entrada constante de novos funcionários, **boa parte permanece tempo suficiente para gerar experiência e cultura organizacional**.
- Os outliers com mais de 20 anos representam **capital histórico e institucional** — valem atenção em políticas de reconhecimento e sucessão.

##### Variável - Anos  no mesmo Cargo
Esta variável é um reflexo da estagnação, evolução de carreira e possíveis riscos de desmotivação dos funcionários do time.

Análises da Composição da Tabela de frequência:
- **55% dos colaboradores estão há no máximo 3 anos no mesmo cargo**.
- **Apenas 7% estão há 10 anos ou mais**, indicando baixa estagnação prolongada.

<div align="center">
<img src= https://github.com/user-attachments/assets/86b257d3-9ef6-4dde-bd24-bc7c92f75390
  alt="Anos no mesmo cargo" width="500" height="300">
  <p><strong> Figura 18:</strong> Boxplot Anos no mesmo cargo.</p>
</div> 

Boxplot — Anos no Mesmo Cargo
Estatísticas visuais extraídas:
- **Mínimo**: 0 anos
- **Q1 (25%)**: 2 anos
- **Mediana**: 3 anos
- **Média**: 4,23 anos
- **Q3 (75%)**: 7 anos
- **Máximo** (sem outliers): 14 anos
- Outliers identificados: 15, 16, 17, 18 ano

*Interpretações e reflexões:*
- **Estrutura dinâmica de movimentação interna**: A maioria dos colaboradores ainda está em períodos iniciais ou intermediários no mesmo cargo — o que indica alta mobilidade interna, seja por promoções ou movimentações laterais.
- **Mediana moderada (3 anos)**: O tempo típico em um cargo é razoável, sem indicar nem rotatividade excessiva nem estagnação.
- **Ponto de atenção estratégico**: Os poucos outliers (acima de 15 anos no mesmo cargo) merecem atenção — **podem representar perfis altamente especializados** ou **estagnados**, com riscos de **desmotivação, baixa inovação** ou perda de capital humano por aposentadoria.

##### Variável - Anos desde a última promoção.

Esta variável é uma excelente métrica para entender ritmo de crescimento interno, política de reconhecimento e possíveis gargalos de progressão de carreira.

Análises da Composição da Tabela de frequência:
- 78,2% foram promovidos nos últimos 3 anos, o que indica uma política forte de mobilidade interna ou crescimento organizacional.
- Apenas 7,3% estão há mais de 7 anos sem promoção, o que pode representar estagnação ou perfis muito seniores.

<div align="center">
<img src= https://github.com/user-attachments/assets/a8f807c7-6b98-4d3a-84a1-189e69581a73
  alt="Anos desde a última promoção" width="500" height="300">
  <p><strong> Figura 19:</strong> Boxplot Anos desde a última promoção.</p>
</div> 

Boxplot — Anos desde a Última Promoção
Estatísticas visuais extraídas:
- **Mínimo**: 0 anos
- **Q1 (25%)**: 0 anos
- **Mediana (Q2)**: 1 ano
- **Média**: ~2,19 anos
- **Q3 (75%)**: 3 anos
- **Máximo** (sem outliers): 7 anos
- **Outliers**: 8, 9, 10, 11, 12, 13, 14 e 15 anos.
  
*Interpretações e reflexões:*
- Distribuição fortemente assimétrica à direita: A maioria dos colaboradores foi promovida recentemente, enquanto há uma cauda longa com poucos profissionais sem promoção há muitos anos — capturados como outliers.
- Mediana de 1 ano confirma um ciclo médio de promoção relativamente rápido -*1 de cada 2 funcionários foram promovido no último ano*
- Os outliers (8 a 15 anos) são casos isolados que merecem atenção:
- São perfis possivelmente estagnados;
- Ou ocupam cargos de topo com menos oportunidades de progressão.

 Conclusão Integrada
>A análise mostra que a empresa apresenta uma dinâmica de promoção recente robusta, com mais de 3 em cada 4 funcionários promovidos nos últimos 3 anos. O boxplot reforça essa concentração no início da distribuição e destaca uma minoria com longos períodos sem ascensão, que pode representar riscos de desengajamento ou baixa mobilidade em posições superiores.

##### Variável - Anos com o mesmo chefe

A variável anos com o mesmo chefe oferece uma leitura muito valiosa sobre **continuidade de lideraça, estabilidade gerencial** e possíveis impactos na cultura e satisfação organizacional.
Com análises da tabela de frequência dos dados podemos checar que:
-  **Mais da metade dos colaboradores (56,1%) está há até 3 anos com o mesmo líder**.
-  Apenas **6,8%** estão há mais de 10 anos com a mesma liderança

<div align="center">
<img src= https://github.com/user-attachments/assets/7f57496a-9d82-4817-afcc-51da26987f46
  alt="Anos com o mesmo chefe width="400" height="200">
  <p><strong> Figura 20:</strong> Boxplot Anos com o mesmo chefe.</p>
</div>

**Boxplot — Anos com o Mesmo Chef**
Estatísticas visuais observadas:
- **Mínimo**: 0 anos
- **Q1 (25%)**: 2 anos
- **Mediana**: 3 anos
- **Média**: 4,12 anos
- **Q3 (75%)**: 7 anos
- **Máximo** (sem outliers): 14 anos
- **Outliers**: 15, 16, 17 anos de liderança contínua

O boxplot mostra distribuição **assimétrica à direita**, com a maioria concentrada nos primeiros anos de relacionamento com o chefe, e poucos casos extremos com tempo de convivência bastante longo.

Tabla 3: Integração — Frequência + Boxplot
| Ponto de Análise                | Evidência na Tabela                  | Representação no Boxplot                  |
|---------------------------------|--------------------------------------|-------------------------------------------|
| Rotatividade / cargos recentes  | 56,1% estão com chefes há ≤ 3 anos   | Bigode inferior e metade inferior da caixa |
| Tempo típico com liderança      | Mediana ≈ 3 anos                     | Centro da caixa (Q2)                      |
| Relacionamentos longevos raros  | 6,8% têm mais de 10 anos com líder   | Outliers (15–17 anos)                     |

*Interpretações e reflexões:*
-  Lideranças relativamente recentes predominam — metade dos colaboradores teve mudança de gestor nos últimos 3 anos. Isso pode indicar:
    - Reestruturações frequentes;
    - Promoções internas e movimentações de liderança;
    - Ou rotatividade de gestores.
-  Mediana de 3 anos mostra que a relação com o gestor direto tende a durar, mas ainda assim renova-se ao longo do tempo.
-  Outliers com 15 a 17 anos com o mesmo líder são perfis raros e podem sinalizar:
    - Equipes muito estáveis;
    - Culturas de longo prazo;
  - Ou riscos de estagnação e resistência à mudança.

#### Análises Univariada. Variáveis Quantitativa Contínua

##### Variável - Salário Mensal dos Funcionários

Considerando as análises da tabela de frequência salarial e do boxplot de salários para tirar conclusões relevantes sobre a distribuição da remuneração mensal na organização temos que:
- Os salários concentram-se entre **R$ 1.600 e R$ 5.599**, com destaque para as faixas **R$ 1.600–3.599** (31,5% da amostra).
- A faixa mais alta (> R$ 10.600) representa **16,9%**, sugerindo um **grupo de alta remuneração ou cargos estratégicos**.

<div align="center">
<img src= https://github.com/user-attachments/assets/a84a5000-f066-4006-8a6a-798e952a7255
  alt="Salário Mensal dos Funcionários width="200" height="400">
  <p><strong> Figura 21:</strong> Boxplot Salário Mensal dos Funcionários.</p>
</div>

**Boxplot — Distribuição Salarial**
Estatísticas visuais observadas:
- **Mínimo**: R$ 1.009,00
- **Q1 (25%)**: R$ 2.910,50
- **Mediana**: R$ 4.919,00
- **Média**: R$ 6.502,93
- **Q3 (75%)**: R$ 8.380,25
- **Máximo** (normal): R$ 18.555,00
- **Outliers**: Salários acima de 18 mil

O intervalo interquartil (Q1–Q3) vai de R$ 2.910,50 a R$ 8.380,25, ou seja, 50% da empresa está dentro dessa faixa.

 Tabla 4: Integração — Tabela + Boxplot
| Ponto de Análise              | Evidência da Tabela                        | Complemento do Boxplot                                 |
|-------------------------------|--------------------------------------------|--------------------------------------------------------|
| Concentração salarial         | 57% ganham entre R$ 1.600 e R$ 5.599       | Mediana = R$ 4.919 confirma foco intermediário         |
| Dispersão e desigualdade      | 17% ganham mais de R$ 10.600               | Média (R$ 6.502) > Mediana (assimetria à direita)      |
| Presença de salários extremos | Pequeno grupo de elite salarial            | Outliers acima de R$ 18 mil evidenciam disparidade     |
 
*Interpretações e reflexões:*
- **Distribuição assimétrica à direita (positiva)**: A média é puxada para cima por um grupo de funcionários com salários bastante elevados — o que **eleva o valor médio** sem alterar a mediana.
- **Alta desigualdade interna**: Há forte variação salarial dentro da empresa, com **boa parte da força de trabalho na base e um grupo seleto no topo**. Isso pode ter reflexos em clima, engajamento e percepção de justiça interna.
- **Faixa intermediária sólida**: O grosso da remuneração está na faixa entre R$ 3 mil e R$ 5,5 mil — base estável que pode ser alvo de políticas de reconhecimento e progressão.

##### Variável - Percentual de Aumento Salarial (2018–2019)

Integrando as análises da tabela de frequência do porcento de aumento salaria (2018-2019) com o boxplot, que revela os padrões de reajuste salarial da empresa — importantíssimo para avaliar justiça interna, reconhecimento e competitividade de mercado.
- Cerca de 56% dos funcionários tiveram aumento entre 11% e 14%
- Apenas 4,6% receberam aumentos mais expressivos (23–25%)

<div align="center">
<img src= "https://github.com/user-attachments/assets/9d1ed09e-fc67-485b-bd7b-6a4fdbb3eaae"
  alt="Percentual de Aumento Salarial (2018–2019) width="500" height="300">
  <p><strong> Figura 22:</strong> Boxplot Percentual de Aumento Salarial (2018–2019).</p>
</div>

**Boxplot — % de Aumento de Salário**
Estatísticas visuais observadas:

- **Mínimo**: 11%
- **Q1 (25%)**: 12%
- **Mediana**: 14%
- **Média**: 15,21%
- **Q3 (75%)**: 18%
- **Máximo** (normal):  25%

O intervalo interquartil vai de 12% a 18%, concentrando metade dos reajustes nesse intervalo.

Tabla 5: Integração — Tabela × Boxplot
| Ponto de Análise | Evidência na Tabela | Complemento do Boxplot | 
|------------------|---------------------|------------------------|
| Aumentos modestos comuns | 55,7% com reajustes entre 11% e 14% | Q1 = 12% confirma concentração à esquerda | 
| Mediana estratégica | Faixa modal entre 13–14% | Mediana = 14% mostra ligeira assimetria à direita | 
| Reajustes generosos (topo) | Apenas 12% acima de 20% | Máximo = 25% sem outliers visíveis | 

*Interpretações e reflexões:*
 -  **Distribuição levemente assimétrica à direita** — a média é um pouco maior que a mediana devido a um pequeno grupo com aumentos mais elevados (23–25%).
 -  **Política de aumento moderada e padronizada**: Mais da metade dos colaboradores recebeu reajustes similares (entre 11–14%), o que pode refletir critérios objetivos e políticas salariais uniformes.
 -  **Baixa dispersão salarial no aumento anual**: O boxplot mostra que quase todos os reajustes ficaram abaixo de 25%, e não há outliers extremos — reforçando coerência na política de meritocracia ou reajuste coletivo.

#### Tabela 6:  Matriz Geral — Perfil de Todos os Funcionários (20 Variáveis)

| Tema                           | Variável                            | Insight Principal                                                                                  |
|--------------------------------|-------------------------------------|----------------------------------------------------------------------------------------------------|
| Perfil Demográfico             | Idade                               | Adultos de 28–42 anos predominam → **força de trabalho madura e ativa**.                           |
|                                | Gênero                              | 60% homens, 40% mulheres → **distribuição levemente masculina**.                                   |
|                                | Estado Civil                        | ~46% casados → **tendência à busca por estabilidade**.                                             |
|                                | Tempo de Carreira                   | 73% com até 14 anos → **perfil em consolidação**.                                                  |
|                                | Quantidade de Empresas              | ~49% com 0–1 empresa → **grande proporção em início de jornada**.                                  |
| Trajetória na Empresa          | Tempo de Empresa                    | Mediana = 5 anos → boa retenção média.                                                             |
|                                | Tempo no Mesmo Cargo                | 55% até 3 anos → alta mobilidade funcional.                                                        |
|                                | Tempo com o Mesmo Chefe             | Mediana de 3 anos → equilíbrio entre continuidade e renovação.                                     |
|                                | Tempo desde Última Promoção         | 64% promovidos nos últimos 2 anos → forte mobilidade interna.                                      |
| Qualificação & Técnico         | Formação Acadêmica                  | 69% com nível superior ou mais → equipe bem qualificada.                                           |
|                                | Qtde de Ações da Empresa            | 43% não possuem ações → engajamento financeiro concentrado.                                        |
|                                | Horas de Treinamento                | ~71% com 2 ou 3h → política de capacitação padronizada e superficial.                              |
| Remuneração & Benefícios       | Salário Mensal                      | Mediana = R$ 4.919; Média = R$ 6.502 → alta disparidade salarial.                                  |
|                                | % Aumento Salarial (2018–2019)      | ~56% entre 11–14% → política salarial padronizada.                                                 |
| Clima & Engajamento            | E-Satisfação (Clima Organizacional) | 61% com satisfação alta/muito alta → clima positivo.                                               |
|                                | Equilíbrio Vida-Trabalho            | 95% com percepção de equilíbrio → ambiente saudável.                                               |
|                                | Faz Horas Extras                    | 28% fazem → potencial sobrecarga em parte da força de trabalho.                                    |
|                                | Frequência de Viagens               | 71% viajam raramente → baixa exposição a deslocamentos.                                            |
| Mobilidade                     | Distância até o Trabalho            | ~64% moram até 9km → logística favorável.                                                          |

#### - Perfil-Padrão de Funcionário com Alta Propensão ao Turnover
Com base aos resultados anteriores podemos construir o **perfil-padrão dos funcionários com maior prospeção a sair da empresa** e, logo depois algumas **recomendações práticas para reteção segmentada** com focos pontos críticos identificados

 Tabela 7: Perfil-Padrão de Funcionário com Alta Propensão ao Turnover
| Dimensão                    | Característica com maior tendência de saída                                      |
|-----------------------------|----------------------------------------------------------------------------------|
| Idade                       | Entre 28 e 37 anos (45% dos desligados)                                          |
| Tempo de empresa            | Até 5 anos (68% dos que saem)                                                    |
| Promoção recente            | 67% saíram após promoção no último ano                                           |
| Salário                     | Até R$ 3.599 (54%)                                                               |
| Satisfação com o clima      | 48,5% tinham satisfação média ou baixa                                           |
| Faz horas extras            | 54% faziam horas extras                                                          |
| Distância até o trabalho    | Mais de 9 km                                                                     |
| Tempo no mesmo cargo        | Até 3 anos                                                                       |
| Ações da empresa            | 65% não tinham ações                                                             |
| Horas de treinamento        | 70% receberam 2 ou 3 horas                                                       |
| Formação                    | Superior e Mestrado (66%)                                                        |

---

###  Etapa 3: Preparação dos Dados

Nesta etapa da metodologia CRISP-DM, o objetivo é transformar os dados brutos em um formato apropriado para análise, garantindo qualidade, consistência e relevância.

####  Estratégia de Preparação

Durante a preparação, aplicamos as seguintes práticas:

- Validação e remoção de duplicidades e registros inconsistentes
- Tratamento de valores ausentes
- Conversão de variáveis categóricas em formato adequado para análise
- Agrupamento de variáveis em faixas (binning) quando necessário
- Padronização de escalas e formatos
---

### Etapa 4: Modelagem

Nesta fase inicial do projeto, optamos por não aplicar modelagem estatística preditiva. O foco esteve em análises descritivas e exploratórias, com o objetivo de compreender os fatores associados ao turnover de funcionários.

####  Tipo de Problema

Trata-se de um problema de **classificação binária**, onde a variável alvo é `Funcionário_deixou_a_empresa` (sim/não). Buscamos identificar os fatores que mais influenciam essa decisão.

####  Abordagens Utilizadas

- Análise de associação entre variáveis categóricas e turnover.
- Aplicação do **Information Value (IV)** para medir o poder de separação das variáveis em relação à variável alvo.
- Avaliação da relação entre turnover e fatores internos da empresa, como tempo de casa, departamento e nível de satisfação.

> Variáveis com IV > 0.3 foram consideradas como fortes candidatas para futuras modelagens preditivas.

<div align="center">
<img src= https://github.com/user-attachments/assets/a87c6338-843a-4d1d-9fcd-c2176b3a86dc
  alt="Framework de Análise de Dado width="600" height="400">
  <p><strong> Figura 23 </strong> Framework de Análise de Dados by Preditiva.ia.</p>
</div>

####  Análise de Associação com a Variável Alvo

Como o foco é entender **quais variáveis influenciam a decisão do funcionário de sair da empresa**, aplicamos técnicas de **medidas de associação**, com destaque para o método **Information Value (IV)**.

####  O que é o Information Value?

O Information Value é uma métrica que indica **o poder preditivo de uma variável categórica ou binned (agrupada) em relação a uma variável alvo binária**. Quanto maior o IV, mais forte é a associação.
Se uma variável tem poder forte, isso significa que uma ou mais categorias da variável tem um alto ou baixo nível de turnover, sendo útil estudá-la com mais profundidade.

Tabela 8:  Valore de *information Value* e sua interpretação

| Valor de IV         | Interpretação                |
|---------------------|------------------------------|
| < 0.02              | Pouco ou nenhum valor preditivo |
| 0.02 - 0.1          | Valor fraco                  |
| 0.1 - 0.3           | Valor médio                  |
| 0.3 - 0.5           | Valor forte                  |
| > 0.5               | Valor suspeito (pode ser overfitting) |

####  Ranking de Variáveis por Information Value

Abaixo está o ranking das principais variáveis associadas com o turnover, com base nos valores de *Information Value* calculados:

Tabela 9:  Variáveis mais signficativas da base conforme o valor de *Information value*

| Variável                   | Information Value | Nível de Associação |
|----------------------------|-------------------|---------------------|
| Salário                    | 0.430             | Forte               |
| Faz_hora_extras?           | 0.400             | Forte               |
| Qte_ações_da_empresa       | 0.319             | Forte               |
| Tempo_de_empresa           | 0.317             | Forte               |
| Idade                      | 0.314             | Forte               |
| Anos_com_o_mesmo_chefe     | 0.263             | Médio               |
| Anos_no_mesmo_cargo        | 0.252             | Médio               |
| Estado_Civil               | 0.219             | Médio               |
| Frequência de Viagens      | 0.121             | Médio               |


> IV permitiu identificar os principais grupos grupos de riscos e as vairáveis com um alto poder separação ao turnover

Esta análise permite focar nos fatores mais relevantes para a saída dos colaboradores, direcionando as próximas etapas do projeto:

- **Modelagem preditiva com as variáveis de maior IV**
- **Proposição de plano de ação para retenção baseado nos fatores de maior impacto**

###  Etapa 5: Avaliação
#### Interpretação dos resultados obtidos apartir do cálculo do *Information Value*.  

 Salário
  - Funcionários com salário baixo têm uma maior taxa de saída.
  - Isso sugere que políticas de remuneração podem ser um fator crítico de retenção.
    
Horas Extras
  - Colaboradores que fazem horas extras tendem a sair mais da empresa.
  - Pode indicar sobrecarga de trabalho ou baixa satisfação.
    
Quantidade de Ações da Empresa
  - Funcionários com menos ações tendem a sair mais.
  - Isso pode indicar que incentivos de participação acionária ajudam na retenção.
    
Tempo de Empresa
  - Funcionários com menos tempo de casa têm maior propensão a sair.
  - Estratégias de **onboarding e engajamento nos primeiros anos** podem ser eficazes.
    
Idade
  - A taxa de turnover é **mais alta entre os mais jovens**.
  - Pode refletir **busca por crescimento rápido** ou **menor estabilidade profissional**.
    

#### Comparação com benchmarks do setor para validar insights.  

Como base as top 5 das variáveis por índice de IV podemos concluir que:

1. Turnover sob controle, mas com margem para melhoria
 - A taxa de 16,1% está **dentro da faixa aceitável para empresas de tecnologia**, mas **acima da média ideal (13%)**.
 - Isso indica que **ações preventivas são recomendadas**, especialmente em áreas com maior risco (ex: salários baixos, sobrecarga, jovens talentos).

2. Validação dos fatores de risco
 - Os fatores identificados no seu projeto (salário, horas extras, tempo de empresa, idade) **refletem os principais motivos de turnover voluntário no Brasil**.
 - Isso reforça a validade dos seus dados e análises.

3. Benchmark como meta
- Podemos definir os 13% como meta de redução para os **próximos 12 meses**.
- Isso pode ser incorporado ao roadmap projeto para futuros analises como critério de sucesso.

####  Conclusão

Esses insights são valiosos para a área de RH e gestão, pois permitem ações direcionadas como:

Reavaliar faixas salariais.
Monitorar e equilibrar a carga de trabalho.
Criar programas de incentivo de longo prazo.
Investir em retenção de talentos jovens e recém-contratados.

---

###  Etapa 6: Implantação

#### Tabela 10: Plano de Ação – Redução de Turnover com base em variáveis críticas

| Prioridade | O que fazer?                                 | Por que?                                                                 | Quem?                              | Como fazer?                                                                                                                                         | Custo Estimado                                      | Horizonte de Tempo     |
|------------|-----------------------------------------------|-------------------------------------------------------------------------|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|------------------------|
| 1          | Revisão da política de Horas Extras           | Colaboradores que fazem hora extra têm maior propensão ao turnover.     | Time de RH e Operações             | Criar grupos de controle e teste. Monitorar impacto com dashboards de turnover e produtividade.                                                     | Possível redução de produtividade em áreas críticas | Curto prazo (0–3 meses) |
| 2          | Revisão Salarial e de Benefícios              | Salário é a variável com maior IV (0.43).                               | Time de Remuneração e Financeiro   | Realizar benchmarking salarial. Avaliar viabilidade de ajustes ou benefícios complementares.                                                        | Aumento da folha de pagamento                        | Médio prazo (3–6 meses) |
| 3          | Programa de Retenção para Novos Colaboradores | Funcionários com pouco tempo de empresa têm maior risco de saída.       | Time de Cultura e Onboarding       | Reforçar onboarding, criar plano de integração de 90 dias, mentorias e acompanhamento com líderes.                                                  | Horas de projeto e treinamento                       | Curto prazo (0–3 meses) |
| 4          | Incentivo à Participação Acionária            | Colaboradores com mais ações tendem a permanecer.                       | Diretoria e RH Estratégico         | Expandir programa de ações para mais níveis hierárquicos. Comunicar benefícios de longo prazo.                                                      | Custo de diluição acionária ou bônus atrelado        | Médio prazo (3–6 meses) |
| 5          | Plano de Desenvolvimento para Jovens Talentos | Jovens têm maior propensão ao turnover.                                 | RH e Desenvolvimento Organizacional | Criar trilhas de carreira, programas de aceleração e feedback contínuo para jovens profissionais.                                                   | Investimento em capacitação e coaching               | Longo prazo (6–12 meses) |
| 6          | Pesquisa de Satisfação e Clima Organizacional | Para entender melhor os motivos subjetivos de saída.                    | RH e Comunicação Interna           | Aplicar pesquisa qualitativa e quantitativa com foco em propósito, cultura e equilíbrio vida-trabalho.                                              | Ferramenta externa de pesquisa ou consultoria        | Curto prazo (0–3 meses) |

####  Métricas para Acompanhamento da Retenção de Funcionários

Acompanhar a retenção de talentos é essencial para avaliar a eficácia das estratégias de RH e reduzir o turnover. Abaixo estão as principais métricas recomendadas:

1. Taxa de Retenção

  **Fórmula:**  Taxa de Retenção = ((Funcionários no final do período - Novas contratações) / Funcionários no início do período) × 100
  **Objetivo:** Avaliar a capacidade da empresa de manter seus colaboradores ao longo do tempo.
  **Periodicidade:** Mensal, trimestral ou anual.

 2. Taxa de Turnover
  Turnover = (Número de desligamentos no período / Número médio de funcionários) × 100
  
  **Objetivo:** Medir a rotatividade geral da empresa.
  **Recomendações:**
  - Segmentar por área, faixa etária, tempo de empresa, tipo de desligamento (voluntário/involuntário).

3. Turnover Voluntário vs. Involuntário

  **Objetivo:** Entender se os desligamentos são motivados por decisão do colaborador ou da empresa.
  
  **Insight:** Altas taxas de turnover voluntário indicam problemas de engajamento, cultura ou liderança.

4. Tempo Médio de Permanência

  **Fórmula:**  Tempo Médio = Soma do tempo de permanência de todos os funcionários desligados / Número de desligamentos
  
  **Objetivo:** Avaliar a longevidade média dos colaboradores na empresa.

5. Índice de Retenção nos Primeiros 12 Meses
    Retenção 12M = (Número de novos contratados que permanecem após 12 meses / Total de contratados no período) × 100
   
      **Objetivo:** Avaliar a eficácia do onboarding e da integração inicial.

7. eNPS (Employee Net Promoter Score)
   **Fórmula:**     eNPS = % Promotores - % Detratores
   
   **Objetivo:** Medir o nível de satisfação e lealdade dos colaboradores.
   
   **Como aplicar:** Pesquisa com a pergunta “Em uma escala de 0 a 10, o quanto você recomendaria esta empresa como um bom lugar para trabalhar?”

9. Absenteísmo
  **Fórmula:** Absenteísmo = (Total de horas/dias de ausência / Total de horas/dias trabalháveis) × 100
   
  **Objetivo:** Pode ser um indicador indireto de desengajamento.

Sugestões de Acompanhamento

- Criar dashboards mensais com gráficos de tendência.
- Estabelecer alertas automáticos para áreas com aumento de turnover.
- Segmentar por perfil (idade, cargo, tempo de empresa, etc.).
- Comparar com benchmarks internos e externos.

##  Referências: 

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
