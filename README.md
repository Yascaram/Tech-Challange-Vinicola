# 🍇 Análise do Mercado Vitivinícola Brasileiro: Produção, Exportação e Importação

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458.svg)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7+-informational.svg)](https://matplotlib.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Este repositório contém uma análise de dados exploratória e quantitativa sobre o setor vitivinícola do Brasil, abrangendo o comportamento histórico e recente dos fluxos de **Exportação**, **Importação** e **Produção** nacional para **Vinhos de Mesa**, **Espumantes** e **Sucos de Uva**.

---

## 📌 Sumário
- [Visão Geral](#-visão-geral)
- [Fontes de Dados](#-fontes-de-dados)
- [Principais Descobertas e Insights](#-principais-descobertas-e-insights)
  - [1. Exportações](#1-exportações)
  - [2. Importações](#2-importações)
  - [3. Produção Nacional de Uva](#3-produção-nacional-de-uva)
- [Estrutura do Repositório](#-estrutura-do-repositório)
- [Como Executar](#-como-executar)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Licença](#-licença)

---

## 📖 Visão Geral

O objetivo deste projeto é diagnosticar a dinâmica comercial e produtiva da vitivinicultura brasileira:
1. **Exportação:** Identificar os principais parceiros comerciais, os destinos líderes em faturamento e volume, e a evolução das categorias exportadas.
2. **Importação:** Analisar o volume e a dependência do mercado interno frente a fornecedores internacionais.
3. **Produção Agrícola:** Mapear a evolução do valor da produção de uva no Brasil e a distribuição geográfica entre os estados produtores.

---

## 📂 Fontes de Dados

Os dados utilizados no projeto são provenientes de fontes públicas e oficiais do setor:
* **Comércio Exterior (Exportação e Importação):** Dados históricos da [Embrapa Uva e Vinho](http://vitibrasil.cnpuv.embrapa.br/).
  * `ExpVinho.csv`, `ExpEspumantes.csv`, `ExpSuco.csv`
  * `ImpVinhos.csv`, `ImpEspumantes.csv`, `ImpSuco.csv`
* **Produção Agrícola Municipal (PAM):** Dados do [IBGE / PAM](https://www.ibge.gov.br/estatisticas/economicas/agricultura-e-pecuaria/9117-producao-agricola-municipal-culturas-temporarias-e-permanentes.html).
  * `uva-valor-da-produo-mil-reais.csv` (Série histórica)
  * `uva-valor-da-produo-2024.csv` (Distribuição estadual)

---

## 📊 Principais Descobertas e Insights

### 1. Exportações
* **Maiores Destinos Históricos Acumulados:**
  * **Volume:** **Estados Unidos** lidera com **135.022.125 kg**.
  * **Faturamento:** **Japão** lidera com **US$ 211.669.661,00** (impulsionado pelo alto valor agregado do suco de uva concentrado).
* **Liderança por Segmento:**
  * **Vinhos de Mesa:** Paraguai (127,58 milhões de kg | US$ 102,72 milhões).
  * **Espumantes:** Estados Unidos (3,97 milhões de kg | US$ 11,21 milhões).
  * **Sucos de Uva:** Japão (95,35 milhões de kg | US$ 203,84 milhões).
* **Tendências Observadas:**
  * *Vinhos de Mesa:* Mercado volátil, com picos históricos de granel em 1993 e 2009. Retomou patamares estáveis de US$ 9 a 11 milhões anuais a partir de 2020.
  * *Espumantes:* Expansão contínua a partir dos anos 2000, batendo recorde de faturamento em 2022 (US$ 2,87 milhões).
  * *Sucos de Uva:* Produto de alta relevância cambial, com recuperação expressiva após 2021, mantendo-se acima de US$ 8 milhões anuais.
* **Ano Mais Recente (2025):** Faturamento total consolidado de **US$ 21,55 milhões** (10,25 milhões de kg exportados).

---

### 2. Importações
* **Volume e Valor:** O **Chile** é o parceiro dominante no mercado brasileiro, acumulando **990.623.107 kg** e **US$ 2,63 bilhões**.
* **Segmentação por Produto:**
  * **Vinhos de Mesa:** Chile é o fornecedor hegemônico com **981.053.253 kg** e **US$ 2,61 bilhões**.
  * **Espumantes:** Liderança da **França** em valor (**US$ 403,03 milhões**), evidenciando a preferência por rótulos de alto valor agregado (Champagne).
  * **Sucos de Uva:** **Argentina** lidera (27,96 milhões de kg | US$ 23,42 milhões).
* **Dinâmica do Mercado:**
  * Forte expansão contínua da importação de vinhos finos e de mesa (>150 milhões de kg/ano nos anos recentes).
  * Redução substancial e residual na importação de sucos, reflexo da consolidação e autossuficiência da indústria nacional de sucos integrais.

---

### 3. Produção Nacional de Uva
* **Crescimento do Valor da Produção (2020–2024):**
  * Salto de **R$ 3,63 bilhões (2020)** para **R$ 8,34 bilhões (2024)**, representando um crescimento acumulado de **+129,78%**.
* **Distribuição Geográfica (2024):**
  * **Pernambuco (Vale do Submédio São Francisco):** Liderança nacional com **51,71%** do valor da produção (**R$ 4,31 bilhões**), impulsionado pelo cultivo irrigado de uvas de mesa para consumo e exportação.
  * **Rio Grande do Sul (Serra Gaúcha):** Responsável por **19,18%** (**R$ 1,60 bilhão**), tradicional polo de vinificação e processamento de sucos.
  * **Bahia:** **11,34%** (R$ 945,22 milhões).
  * **São Paulo:** **10,51%** (R$ 875,75 milhões).
  * **Paraná:** **3,45%** (R$ 287,37 milhões).

---

## 📁 Estrutura do Repositório

```text
├── data/
│   ├── ExpVinho.csv
│   ├── ExpEspumantes.csv
│   ├── ExpSuco.csv
│   ├── ImpVinhos.csv
│   ├── ImpEspumantes.csv
│   ├── ImpSuco.csv
│   ├── uva-valor-da-produo-mil-reais.csv
│   └── uva-valor-da-produo-2024.csv
├── notebooks/
│   └── tech_sub1.ipynb
├── requirements.txt
├── .gitignore
└── README.md
