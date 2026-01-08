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


## Conclusão e Recomendação Estratégica de Investimento em Marketing (
Após analisar profundamente as métricas de CLV (Customer Lifetime Value), CAC (Customer Acquisition Cost) e ROI (Return on Investment) das diferentes origens de tráfego, fica claro que a Y.Afisha possui um canal de aquisição altamente lucrativo, mas ainda longe de operar no seu potencial máximo devido à distribuição ineficiente do orçamento de marketing. Em outras palavras: os melhores canais têm espaço para escalar e continuar entregando movimento financeiro saudável, enquanto os mais caros drenam orçamento e precisam ser reavaliados.

A partir dos resultados, proponho uma estratégia direta e sustentável. Minhas recomendações são redirecionar parte do investimento para os canais mais eficientes e escalar aquilo que já demonstra, de forma consistente, maior retorno por dinheiro investido.

Minha conclusão final é direta e apoiada pelos dados. É hora de escalar o que funciona e repensar o que drena recursos.

As origens mais eficientes, equivalentes ao que, no mercado, vemos em canais como Google Search Ads com intenção alta, campanhas de retargeting no Meta, influenciadores de nicho, SEO e conteúdo orgânico, e-mail marketing automatizado e marketplaces como Sympla ou Ingressos.com, seguem uma lógica semelhante: baixo custo de aquisição, retorno rápido e alta previsibilidade. São canais que convertem porque o usuário já chega mais quente, mais preparado para a compra e com menor dispersão de atenção. Esses são exatamente os comportamentos observados nas origens 4, 5, 9 e 10 deste projeto analítico. Por isso, faz sentido direcionar mais verba para esse grupo: eles entregam escala com controle e sustentam um crescimento saudável.

Por outro lado, as origens 1, 2 e 3 lembram os canais que, na prática, costumam elevar o CAC sem garantir retorno proporcional: display genérico, campanhas amplas de alcance no Meta, influenciadores grandes demais para o nicho, ou até mídia tradicional quando o produto é digital-first. São investimentos que brilham pela visibilidade, mas nem sempre pelo resultado, e nos dados, esse padrão se repete. Aqui a recomendação é mitigar, testar e reavaliar, evitando desperdiçar capital em canais que já provaram ter eficiência inferior.

Por fim, transformar dados em lucro contínuo exige estratégia, e isso significa operar o marketing como um portfólio vivo. Ajustes mensais com base no ROI, aumento gradual do orçamento nos canais que superam a meta e cortes inteligentes nos que não entregam; ações de pós-venda para elevar o LTV; testes A/B constantes para ampliar a escala sem perder eficiência; criativos mais orientados à performance para reduzir CAC; expansão por lookalike audiences a partir dos clientes de maior valor; e acompanhamento mensal por coortes para detectar rapidamente quando um canal começa a perder força.

A empresa Y.Afisha tem um enorme potencial de crescimento sustentado. Com a realocação adequada, ou seja, menos gasto onde dói e mais investimento onde rende, a empresa pode maximizar o retorno do marketing, reduzir risco operacional e fortalecer o ciclo de aquisição de clientes.

Em resumo, o caminho para maximizar a lucratividade não é gastar mais, e sim gastar melhor, ampliando os canais mencionados acima que comprovadamente geram valor e ajustando aqueles que não acompanham a performance esperada. Essa é a base de uma operação de marketing mais inteligente, sustentável e competitiva.



