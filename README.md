# D1---Ciencia-e-Governanca-de-Dados-

1. Introdução O presente trabalho tem como objetivo a realização de uma análise de dados com foco na compreensão das relações entre o Produto Interno Bruto (PIB) per capita, a expectativa de vida e a taxa de mortalidade de diferentes países. A partir desses indicadores, busca-se identificar padrões que evidenciem como o desenvolvimento econômico pode influenciar diretamente na qualidade e nas condições de vida da população.

A análise foi conduzida em ambiente Python, com a utilização de bibliotecas amplamente reconhecidas na comunidade científica e de ciência de dados, como Pandas, NumPy, Matplotlib e Seaborn.

2. Aquisição dos Dados Os dados utilizados neste estudo foram obtidos a partir de bases públicas de indicadores socioeconômicos e de saúde, contendo informações consolidadas sobre diversos países. As variáveis selecionadas representam medidas relevantes para avaliar o desenvolvimento humano sob perspectivas econômicas e sociais.

O conjunto de dados inclui as seguintes variáveis:

País
PIB per capita (em dólares americanos)
Expectativa de vida (em anos)
Taxa de mortalidade (a cada 100 mil habitantes)
Os arquivos de dados foram armazenados no formato CSV e inseridos no ambiente de execução do notebook, permitindo o tratamento e análise de forma reprodutível e transparente.

3. Metodologia de Aquisição

O conjunto de dados foi construído com base em fontes oficiais e reconhecidas de estatísticas socioeconômicas e de segurança pública no Brasil. Ele inclui três indicadores principais por Unidade da Federação (UF): Produto Interno Bruto (PIB) per capita, taxa de homicídios por 100 mil habitantes e taxa de mortalidade geral.

a) PIB per capita (2022) Os valores de PIB per capita foram obtidos do Instituto Brasileiro de Geografia e Estatística (IBGE), com base nas Contas Regionais de 2022, divulgadas pela Agência de Notícias IBGE. Os dados refletem o valor médio do PIB dividido pela população residente em cada estado, expresso em reais correntes (R$).

Fonte: IBGE – Contas Regionais do Brasil 2022. Link: https://agenciadenoticias.ibge.gov.br/

b) Taxa de homicídios (2023) As estimativas das taxas de homicídio por 100 mil habitantes foram baseadas no Atlas da Violência 2024, publicado pelo Instituto de Pesquisa Econômica Aplicada (IPEA) e pelo Fórum Brasileiro de Segurança Pública (FBSP). Foram utilizadas as taxas estaduais mais recentes disponíveis, representando o ano-base de 2023.

Fonte: IPEA / FBSP – Atlas da Violência 2024. Link: https://www.ipea.gov.br/atlasviolencia/

c) Taxa de mortalidade geral (estimada, 2023) As taxas de mortalidade foram estimadas a partir das Tábuas Completas de Mortalidade do IBGE e complementadas com dados do DATASUS (Ministério da Saúde). Os valores indicam a taxa bruta de mortalidade (óbitos por mil habitantes) por estado.

Fonte: IBGE – Tábuas Completas de Mortalidade 2023; DATASUS / Ministério da Saúde. Links:

https://www.ibge.gov.br/estatisticas/sociais/populacao/
https://datasus.saude.gov.br/
d) Consolidação dos dado Os valores foram organizados em planilha (.csv) com as seguintes colunas:

state: Nome do estado
uf: Sigla da Unidade da Federação
pib_per_capita_2022_R$: Valor do PIB per capita em reais correntes
homicides_per_100k_est_2023: Taxa estimada de homicídios por 100 mil habitantes
mortality_per_1000_est: Taxa estimada de mortalidade geral por mil habitantes
notes: Comentários sobre a origem e eventuais ajustes
4. Principais Etapas do Notebook O notebook foi estruturado de forma sequencial e lógica, seguindo o fluxo tradicional de uma análise exploratória de dados. As principais etapas estão descritas a seguir:

-Carregamento das Bibliotecas As bibliotecas Pandas, NumPy, Matplotlib e Seaborn foram importadas, permitindo a manipulação, análise e visualização dos dados de forma eficiente.

-Leitura e Inspeção Inicial dos Dados O arquivo CSV contendo as variáveis socioeconômicas foi lido e inspecionado, com a finalidade de compreender sua estrutura, identificar possíveis inconsistências e obter uma visão geral das informações disponíveis.

-Tratamento e Limpeza dos Dados Nesta etapa, foram removidos registros com valores ausentes ou inconsistentes, além de realizadas correções de formatação e adequações nas unidades das variáveis.

-Análise Descritiva e Estatística Foram calculadas medidas estatísticas básicas, como média, mediana, desvio-padrão, valores mínimos e máximos, permitindo uma compreensão inicial da distribuição dos dados e identificação de possíveis outliers.

-Visualizações Exploratórias Foram construídos diferentes tipos de gráficos para auxiliar na interpretação dos padrões e relações entre as variáveis. Entre as principais visualizações desenvolvidas, destacam-se: Gráfico de dispersão entre PIB per capita e expectativa de vida, com o intuito de verificar a correlação entre prosperidade econômica e longevidade populacional; Gráfico de dispersão entre PIB per capita e taxa de mortalidade, com o objetivo de avaliar se países mais ricos apresentam menores índices de mortalidade; Histogramas e boxplots para analisar a distribuição das variáveis e a presença de possíveis valores extremos.

5. Interpretação dos Resultados Com base nas análises gráficas e estatísticas, foi possível observar tendências claras entre o PIB per capita e os indicadores de saúde. Países com maior renda per capita apresentaram, em geral, maior expectativa de vida e menores taxas de mortalidade.

Os principais insights extraídos da análise incluem:

Existe uma correlação positiva entre PIB per capita e expectativa de vida, indicando que o desenvolvimento econômico tende a favorecer melhores condições de saúde e longevidade.
Observou-se uma correlação inversa entre PIB per capita e taxa de mortalidade, evidenciando que países com maior renda possuem menor incidência de mortes por causas gerais.
As disparidades regionais e econômicas refletem diretamente na qualidade de vida da população, sendo o PIB um indicador fortemente associado a melhores resultados em saúde pública.

**6. Conclusão** A análise exploratória permitiu compreender de forma aprofundada como o nível econômico de um país influencia indicadores fundamentais de saúde pública. As visualizações e as estatísticas apresentadas reforçam a importância de políticas públicas voltadas à equidade social e ao desenvolvimento sustentável. O estudo demonstra a aplicabilidade da análise de dados como ferramenta essencial para subsidiar tomadas de decisão baseadas em evidências.
