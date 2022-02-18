# SAP

## Introdução

### Objetivo

O SAP centraliza o gerenciamento de dados, assim é possível fornecer várias funções de negócios com apenas uma visão da verdade, evitando duplicidade de dados.

Isso ajuda as empresas a gerenciar melhor os processos de negócios complexos. Distribuindo insights entre diferentes departamentos.

> A linguagem utilizada pelo SAP é o ABAP (Sintaxe parecida com a do COBOL)

### Data Warehouse

Data Warehouse é um repositório central de informações que podem ser analisadas para tomar decisões adequadas. 

Os dados de um Data Warehouse podem vir de Sistemas Transacionais, Banco de Dados Relacionais ou outras fontes.

- OLTP - On-Line ***Transaction*** Processing (ERP)

    - Ambiente transacional com foco operacional, os dados que contém nesse ambiente são detalhados e transacionais, mudam constantemente com eventos de negócio.

- OLAP - On-Line ***Analytical*** Processing (DW)

    - Ambiente analítico com foco estratégico, os dados que contém nesse ambiente são sumarizados e são históricos fixos num ponto específico de tempo e estruturados para queries.

### SAP BW

O BW é um Data Warehouse que, geralmente, busca as informações a partir do ECC.

O BW possui alguns ambientes: 

- Desenvolvimento   -> B1D
- Qualidade         -> B1Q
- Produção          -> B1P

### Tipos de dados 

Existem dois tipos de dados que precisam ser carregados no BW: Dados Mestres e Dados Transacionais.

#### Dados Mestre / Master Data


* armazenados em InfoObjetos;

* Atributos, hierarquias e textos

* Correspondem aos Dados Mestre no SAP;

> Exemplo: Cliente, carro, etc.

#### Dados Transacionais / Transactional Data

* armazenados em InfoCubos e DSO's

* utilizados para análise, ou seja, são dados de movimento extraidos de DataSources

> Exemplo: Criação de pedidos

### Fluxo de cargas no BW