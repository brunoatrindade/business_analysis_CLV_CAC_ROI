# Análise de Negócio: CLV, CAC e ROI

## Visão Geral do Projeto
Este projeto foi desenvolvido como um **estudo de análise de negócio** para a empresa **Y.Afisha**, com o objetivo de **otimizar a eficiência dos investimentos em marketing** 
e maximizar o **Retorno sobre o Investimento (ROI)**.

A análise utiliza dados reais do período de **janeiro de 2017 a dezembro de 2018**, cobrindo toda a jornada do cliente, desde o uso do produto e aquisição por canais de marketing
até a conversão em receita e geração de valor ao longo do tempo.

O projeto foi implementado em **Jupyter Notebook**, combinando **análise exploratória de dados**, **visualizações estratégicas** e **métricas de negócio** para apoiar decisões de 
marketing orientadas por dados.

---

## Objetivos de Negócio
Os principais objetivos desta análise são:

- Entender **como os usuários utilizam o produto**
- Identificar **quando os usuários se tornam clientes pagantes**
- Medir **quanto valor cada cliente gera ao longo do tempo (CLV/LTV)**
- Calcular o **Custo de Aquisição de Clientes (CAC)** por origem
- Determinar o **ponto de equilíbrio** para cobrir os custos de marketing
- Avaliar o **ROI por canal de aquisição**
- Fornecer **recomendações estratégicas** para otimização dos investimentos em marketing

---

## Fontes de Dados
A análise é baseada em três conjuntos de dados principais:

### 1. Logs de Acesso ao Site
**Arquivo:** `/datasets/visits_log_us.csv`

| Coluna | Descrição |
|------|-----------|
| `Uid` | Identificador único do usuário |
| `Device` | Dispositivo utilizado |
| `Start Ts` | Data e hora de início da sessão |
| `End Ts` | Data e hora de término da sessão |
| `Source Id` | Identificador da origem do anúncio |

---

### 2. Dados de Pedidos
**Arquivo:** `/datasets/orders_log_us.csv`

| Coluna | Descrição |
|------|-----------|
| `Uid` | Identificador único do usuário |
| `Buy Ts` | Data e hora do pedido |
| `Revenue` | Receita gerada pelo pedido |

---

### 3. Despesas com Marketing
**Arquivo:** `/datasets/costs_us.csv`

| Coluna | Descrição |
|------|-----------|
| `source_id` | Identificador da origem de marketing |
| `dt` | Data |
| `costs` | Despesas diárias com marketing por origem |

---

## Estrutura da Análise

### Etapa 1 — Preparação dos Dados
- Carregamento dos dados em variáveis Python
- Tratamento e otimização dos tipos de dados
- Garantia de consistência e qualidade para análise
- Preparação das tabelas para métricas e visualizações

---

### Etapa 2 — Relatórios e Métricas

#### Produto
- Usuários ativos diários, semanais e mensais (DAU / WAU / MAU)
- Número de sessões por dia
- Análise da duração das sessões
- Frequência de retorno dos usuários

#### Vendas
- Análise do tempo entre registro e primeira compra (conversão)
- Comparação de conversões por coorte
- Número de pedidos por cliente
- Valor médio de pedido (AOV)
- Cálculo do **Customer Lifetime Value (CLV / LTV)**

#### Marketing
- Total investido em marketing ao longo do tempo
- Investimento por origem de aquisição
- **CAC por canal**
- Avaliação do **ROI por origem de marketing**

Foram construídos gráficos para analisar diferenças por:
- Dispositivo
- Origem de tráfego
- Evolução temporal das métricas

---

### Etapa 3 — Conclusões e Recomendações
Com base nos resultados obtidos, o projeto apresenta:

- Identificação das **origens de marketing mais eficientes**
- Comparação entre **CLV e CAC por canal**
- Análise do **ponto de equilíbrio dos investimentos**
- Recomendações práticas para:
  - Redirecionar investimentos
  - Priorizar canais com maior retorno
  - Otimizar campanhas com baixo desempenho

As conclusões são fundamentadas em métricas financeiras e de comportamento do usuário, visando **maximizar eficiência e sustentabilidade do negócio**.

---

## Ferramentas e Tecnologias
- **Python**
- **Jupyter Notebook**
- **Pandas** — manipulação e análise de dados
- **NumPy** — cálculos numéricos
- **Matplotlib / Seaborn** — visualização de dados
- Técnicas de **análise de coortes e funil**
- Métricas de negócio: **CLV, CAC, ROI e Break-even**

---

## Critérios Atendidos
Este projeto demonstra:

- Preparação e organização adequada dos dados
- Construção de visualizações relevantes
- Cálculo correto e interpretação das métricas
- Raciocínio orientado a negócio
- Código bem estruturado e documentado
- Conclusões claras e acionáveis

---

## Principal Insight
Este projeto evidencia uma abordagem de **Data Analytics orientada a negócio**, onde os dados são utilizados não apenas para análise, mas como base para 
**decisões estratégicas de marketing e crescimento sustentável**.
