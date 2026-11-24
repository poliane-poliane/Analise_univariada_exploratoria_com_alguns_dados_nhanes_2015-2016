# Análise Univariada Exploratória — NHANES (2015–2016)

Este repositório contém um notebook de estudos e referência prática sobre **Análise Exploratória de Dados (EDA) Univariada**, utilizando dados reais da pesquisa **NHANES** (*National Health and Nutrition Examination Survey*) referente ao ciclo de 2015–2016.

## Objetivo

Consolidar técnicas fundamentais de manipulação, limpeza, resumo estatístico e visualização de dados em Python, servindo tanto como material de consulta rápida quanto como guia prático para análise de variáveis categóricas e quantitativas.

## Estrutura do Repositório

- `Analise_Univariada_NHANES.ipynb`: Notebook principal contendo as explicações teóricas, códigos comentados e visualizações gráficas.
- `analise_univariada_nhanes.py`: Script Python equivalente com o fluxo de análise.

## Tecnologias e Bibliotecas Utilizadas

- **Python 3**
- **Pandas & NumPy:** Manipulação de DataFrames, tratamento de valores ausentes (`NaN`), recodificação de categorias e cálculos estatísticos.
- **Matplotlib & Seaborn:** Construção de histogramas, boxplots e gráficos de distribuição.
- **Requests & BeautifulSoup4:** *Web scraping* automatizado diretamente da documentação oficial do CDC para construção do dicionário de dados.

## Conteúdos Abordados no Notebook

1. **Automação de Metadados (Dicionário de Dados):**
   - Extração dinâmica das descrições das variáveis diretamente das páginas oficiais do CDC (`DEMO_I`, `BMX_I`, `BPX_I`, `SMQ_I`, `ALQ_I`).
2. **Manipulação e Limpeza com Pandas:**
   - Leitura e inspeção inicial do dataset (`head()`, `shape`, `columns`, `dtypes`).
   - Diferentes formas de seleção de colunas e fatiamento de dados (`loc`, `iloc`).
   - Criação de cópias seguras (`copy()`) e exclusão de colunas (`drop()`).
   - Mapeamento e tradução de códigos numéricos para rótulos legíveis (`replace()`).
3. **Análise de Variáveis Categóricas:**
   - Tabelas de frequência absoluta e relativa (`value_counts()`, `normalize=True`).
   - Tratamento e contabilização de dados faltantes (`dropna=False`, `fillna()`).
4. **Análise de Variáveis Quantitativas e Resumos Estatísticos:**
   - Medidas de tendência central e dispersão (`describe()`, média, mediana, desvio padrão e intervalo interquartil).
   - Cálculo de proporções condicionais (ex.: prevalência de pré-hipertensão sistólica).
5. **Visualização e Estratificação:**
   - **Histogramas** (`sns.histplot`) para análise de assimetria e formato das distribuições.
   - **Boxplots** (`sns.boxplot`) para identificação de *outliers* e comparação entre grupos.
   - **Estratificação por Faixas Etárias** (`pd.cut()`) para observar variações de comportamento em subgrupos populacionais.

## Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/SEU-USUARIO/Analise_univariada_exploratoria_com_alguns_dados_nhanes_2015-2016.git
