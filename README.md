# Análise do Desempenho Comercial e Oportunidades de Crescimento no E-commerce

## Sobre o projeto

Este projeto foi desenvolvido como parte do Tech Challenge da Pós-Tech em Data Analytics da FIAP e tem como objetivo analisar o desempenho comercial das categorias de produtos do ecossistema de e-commerce da Olist.

A partir da integração e análise de dados de pedidos, itens comercializados, produtos e avaliações de consumidores, busca-se identificar categorias com indicadores promissores de crescimento comercial e satisfação dos clientes.

## Pergunta de negócio

**Quais categorias de produtos apresentam crescimento de valor comercializado acima do crescimento geral e mantêm bons níveis de satisfação dos clientes?**

## Base de dados

Foi utilizado o *Brazilian E-Commerce Public Dataset by Olist*, um conjunto de dados público e anonimizado que reúne informações sobre pedidos realizados em uma plataforma de e-commerce brasileira.

Fonte: [Brazilian E-Commerce Public Dataset – Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

Foram utilizadas as seguintes bases:

- `olist_orders_dataset.csv`: informações dos pedidos.
- `olist_order_items_dataset.csv`: itens associados aos pedidos.
- `olist_products_dataset.csv`: informações e categorias dos produtos.
- `olist_order_reviews_dataset.csv`: avaliações dos consumidores.
- `olist_sellers_dataset.csv`: informações dos vendedores, utilizadas como apoio na verificação de integridade dos dados.

## Metodologia

A análise foi desenvolvida em Python, utilizando técnicas de exploração, tratamento, integração e visualização de dados.

Foram considerados pedidos com status `delivered`, realizados entre janeiro de 2017 e junho de 2018.

Para avaliar a evolução comercial, foram comparados os primeiros semestres de 2017 e 2018, utilizando indicadores como:

- Valor comercializado em produtos.
- Crescimento percentual por categoria.
- Participação das categorias no valor total comercializado.
- Variação de participação de mercado, em pontos percentuais.

A análise de satisfação considerou as avaliações associadas aos pedidos que continham produtos de cada categoria, observando a nota média, o percentual de avaliações positivas e negativas e o volume de pedidos avaliados.

## Ferramentas e tecnologias

- **Python:** linguagem utilizada no desenvolvimento da análise.
- **Pandas e NumPy:** manipulação, tratamento e análise dos dados.
- **Matplotlib e Seaborn:** construção e personalização das visualizações.
- **Google Colab / Jupyter Notebook:** ambiente de desenvolvimento.

## Principais resultados

A análise identificou diferentes padrões de desempenho entre as categorias:

- **Beleza e Saúde:** combinou crescimento comercial, ganho de participação no ecossistema e indicadores de satisfação acima da referência geral, destacando-se como uma oportunidade de expansão.
- **Relógios e Presentes:** apresentou ganho expressivo de participação, acompanhado de crescimento comercial, mas com indicadores de satisfação que merecem atenção.
- **Bebês:** apresentou crescimento acelerado e ganho de participação, embora ainda tenha menor escala comercial.
- **Construção e Ferramentas:** apresentou crescimento percentual elevado e ganho de participação, partindo de uma base inicial pequena.
- **Cama, Mesa e Banho:** destacou-se pelo volume comercial, mas apresentou percentual de avaliações negativas superior à média do ecossistema.

## Estrutura do repositório

```text
├── README.md
├── Tech_Challenge_1.ipynb
└── Dataset.zip
```

*Observação: os arquivos CSV devem estar disponíveis no ambiente de execução para que o notebook possa ser executado integralmente.*

## Como executar o projeto

1. Faça o download do notebook disponível neste repositório.
2. Obtenha os arquivos da base de dados pelo link do Kaggle.
3. Disponibilize os cinco arquivos CSV no diretório de execução do notebook.
4. Abra o notebook no Google Colab ou em um ambiente Jupyter com as bibliotecas necessárias instaladas.
5. Execute as células em sequência para reproduzir as análises e visualizações.

---

**Projeto desenvolvido para o Tech Challenge — Pós-Tech em Data Analytics | FIAP.**
