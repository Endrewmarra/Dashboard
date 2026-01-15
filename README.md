# 📊 Dashboard de Assinaturas — Análise Temporal no Excel

## 📌 Visão Geral

Este repositório contém um projeto de **dashboard interativo desenvolvido em Microsoft Excel**, com foco na **análise temporal de assinaturas**.

O objetivo é demonstrar a capacidade de:
- Organizar dados
- Criar análises temporais
- Construir dashboards interativos
- Aplicar boas práticas de separação entre dados, cálculos e visualização

O resultado final é um **arquivo Excel (.xlsx)** com dashboard funcional e filtros dinâmicos.

---

## 🎯 Objetivo do Projeto

- Analisar a **evolução mensal de assinaturas**
- Avaliar a **variação de receita ao longo do tempo**
- Permitir a **segmentação por tipo de assinatura**:
  - Monthly
  - Quarterly
  - Annual
- Apresentar informações de forma clara, visual e interativa

---

## 🗂️ Estrutura do Arquivo Excel

O arquivo Excel está organizado nas seguintes abas:

### 🔹 `Bases`
Contém a **base de dados original**, utilizada como fonte para todas as análises.

Essa aba reúne informações como:
- Identificação do assinante
- Data de início da assinatura
- Tipo de assinatura (Monthly / Quarterly / Annual)
- Valores associados à assinatura

> ⚠️ Esta aba não deve ser alterada, pois serve como base única de dados.

---

### 🔹 `Cálculos`
Aba responsável por toda a **lógica do projeto**.

Inclui:
- Tabelas Dinâmicas para agregação dos dados
- Cálculo de métricas temporais (ex.: assinaturas por mês, receita mensal)
- Tabelas auxiliares com fórmulas (“tabelas espelho”), utilizadas para alimentar gráficos estáveis

Essa abordagem garante:
- Melhor controle do eixo temporal
- Compatibilidade com filtros (segmentadores)
- Facilidade de manutenção

---

### 🔹 `Assets`
Aba utilizada para armazenar **elementos visuais**, como cores e componentes gráficos de apoio ao layout do dashboard.

---

### 🔹 `Dashboard`
Camada final de visualização.

Contém:
- Gráficos de linha e barras
- Segmentadores de dados (slicers)
- Layout organizado para análise executiva

Todos os gráficos são atualizados automaticamente conforme os filtros aplicados.

---

## 📊 Funcionalidades do Dashboard

- 📈 Análise temporal de assinaturas
- 💰 Visualização da receita ao longo do tempo
- 🎛️ Filtro por tipo de assinatura
- 🔄 Atualização dinâmica dos gráficos conforme a segmentação

---

## 🎛️ Interatividade

O dashboard utiliza **Segmentadores de Dados** para permitir a filtragem por tipo de assinatura.

Os filtros estão conectados às tabelas dinâmicas responsáveis pelos cálculos, garantindo que:
- Os dados sejam atualizados corretamente
- As visualizações permaneçam consistentes
- O eixo temporal dos gráficos seja preservado

---

## 🧠 Decisões Técnicas

Durante o desenvolvimento, foram adotadas as seguintes práticas:

- Uso de **Tabelas Dinâmicas** para cálculos e agregações
- Uso de **gráficos tradicionais (não PivotCharts)** para séries temporais
  - Evita inconsistências no eixo de tempo
  - Garante maior estabilidade visual
- Separação clara entre:
  - Dados (`Bases`)
  - Lógica (`Cálculos`)
  - Visualização (`Dashboard`)

Essas decisões seguem padrões comuns em projetos reais de análise de dados.

---

## ▶️ Como Reproduzir o Projeto

1. Clone este repositório:
   ```bash
   git clone <url-do-repositorio>
   ```
2. Abra o arquivo Excel (.xlsx) presente no repositório
3. Navegue até a aba Dashboard
4. Utilize os filtros disponíveis para interagir com as análises
   - Não é necessário instalar dependências adicionais.

--

## 📌 Tecnologias Utilizadas

- Microsoft Excel
- Tabelas Dinâmicas
- Gráficos
- Segmentadores de Dados
- Fórmulas nativas do Excel

---

##

📈 Possíveis Evoluções

- Inclusão de KPIs adicionais
- Análise de crescimento acumulado
- Novos filtros (ex.: plano, add-ons)
- Migração da lógica para Power BI ou Python

---
