# 🗄️ Projetos de Banco de Dados: Modelagem & SQL

> Repositório monorepo contendo dois projetos acadêmicos completos de Banco de Dados. O foco é demonstrar o ciclo de vida do dado: desde a modelagem conceitual (MER) até a extração de inteligência de negócio com queries complexas em SQL.

<div align="center">

  ![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
  ![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
  ![Database](https://img.shields.io/badge/Database-Modeling-gray?style=for-the-badge&logo=databricks&logoColor=white)

</div>

---

## 🏙️ Projeto 1: Sistema de Gestão Imobiliária

Um banco de dados robusto desenhado para gerenciar o ecossistema complexo de uma imobiliária, controlando vendas, aluguéis e a manutenção dos imóveis.

### ✨ Regras de Negócio & Funcionalidades

O diferencial deste projeto é a implementação de **regras de negócio estritas** via modelagem, como a obrigatoriedade de visitas antes de contratos.

| Módulo | Descrição |
| :--- | :--- |
| 🤝 **Negócios** | Fluxo estruturado: `Visita` ➔ `Proposta` ➔ `Contrato` (Venda ou Aluguel). |
| 📅 **Visitas** | Registro detalhado com feedback do cliente (ex: "Negócio Fechado", "Em dúvida"). |
| 🛠️ **Manutenção** | Controle de vistorias periódicas e reparos necessários nos imóveis. |
| 💰 **Financeiro** | Histórico de pagamentos de aluguéis e comissões de corretores. |

### 📂 Estrutura dos Arquivos

* `MER.png` / `MR.jpg`: Diagramas Conceitual e Lógico.
* `DDL_Imobiliaria.sql`: Criação das tabelas e *constraints*.
* `DML-Imobiliaria.sql`: Massa de dados para testes de carga.
* `Respostas_Imobiliaria.sql`: **28 Queries Analíticas**, respondendo perguntas como:
    * *Quem é o corretor com maior taxa de conversão?*
    * *Qual imóvel é muito visitado mas nunca é vendido ("encalhado")?*
    * *Relatório de faturamento mensal segmentado.*

---

## 🚗 Projeto 2: Locadora de Veículos

Um sistema focado na eficiência operacional, registrando a rotatividade da frota e o comportamento dos clientes.

### ✨ Funcionalidades
* **Gestão de Frota:** Controle total dos veículos disponíveis.
* **Cálculo de Rodagem:** O sistema armazena e calcula a quilometragem percorrida em cada transação.
* **Histórico:** Rastreabilidade de qual cliente utilizou qual carro e em qual período.

### 📂 Estrutura dos Arquivos

* `01-LocadoraCarro-MER.png` e `MR`: Modelagem visual.
* `03-LocadoraCarros-DDL.sql`: Script de definição do esquema.
* `04-LocadoraCarros-DML1.sql`: Inserção de dados.
* `05-LocadoraCarros-DQL.sql`: Relatórios gerenciais (ex: Total de locações por modelo de carro).

---

## 🛠️ Tecnologias Utilizadas

<div align="left">
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-Language-gray?style=for-the-badge" />
  <img src="https://img.shields.io/badge/brModelo-Modeling-gray?style=for-the-badge&logo=creativetim&logoColor=white" />
</div>


