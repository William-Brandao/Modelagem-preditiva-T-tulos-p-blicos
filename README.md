# 📈 Previsão de Marcação a Mercado e Estratégia de Alocação em Títulos Públicos

![badge](https://img.shields.io/badge/status-concluded-brightgreen) ![license](https://img.shields.io/badge/license-MIT-blue) ![python](https://img.shields.io/badge/python-3.10+-blue)

> Projeto de ciência de dados e engenharia de machine learning voltado à previsão do comportamento dos preços dos títulos públicos (Tesouro Direto), com foco em tomada de decisão para alocação de capital em cenários macroeconômicos dinâmicos.

---

## 🚀 Visão Geral

Este projeto desenvolve uma **pipeline preditiva e automatizada**, com foco em **prever se os preços dos títulos públicos terão valorização ou desvalorização** no trimestre seguinte. A partir dessas previsões, é feita uma **alocação estratégica entre títulos curtos, médios e longos**.

O produto final é um **relatório PDF automatizado** com visualizações, métricas e decisões recomendadas — pronto para uso por analistas, gestores e investidores.

---

## 🧠 Metodologia

### 📌 Dados Utilizados
- Títulos públicos: Tesouro IPCA+, Prefixado e Selic (marcação a mercado)
- Variáveis macroeconômicas:
  - IPCA, IGP-M, INCC
  - PIB trimestral, taxa de desemprego, renda média
  - SELIC e metas
  - Fed Funds Rate, inflação EUA, preço do petróleo
  - Indicadores fiscais: dívida/PIB, receita/PIB, termos de troca

### 🔧 Pipeline do Projeto
1. **Coleta e integração automática** dos dados via APIs e bases públicas
2. **Pré-processamento robusto** com tratamento de outliers, missing e normalização
3. **Geração de features temporais, macroeconômicas e derivadas**
4. **Modelagem Preditiva Binária**
   - Classificadores temporais com validação walk-forward
   - Avaliação com métricas como ROC AUC, acurácia, F1
5. **Estratégia de Alocação Dinâmica**
   - Alocação entre vencimentos (curto, médio, longo) baseada em probabilidades previstas
6. **Relatório Final Automatizado**
   - Geração de PDF com gráficos, retornos comparados e drawdown

---

## 📊 Resultados

- **Retorno total acumulado** superior aos benchmarks (CDI, SELIC + IPCA e Ibovespa)
- **Drawdown máximo controlado** (modelo opera com risco reduzido)
- **Melhor desempenho em ciclos de estresse**, como pandemia ou choques externos

### 🖼️ Exemplos de Gráficos:
- Retorno percentual anual por estratégia
- Drawdown acumulado
- Alocação por período
- Correlação entre variáveis macroeconômicas

---

## 🧾 Avaliação Profissional

> **Média final**: `93.78/100`  
> **Classificação**: `Sênior – Pronto para produção`  
> Avaliado com critérios como organização do código, automação, documentação e entrega de valor.

---

## 🛠️ Tecnologias e Ferramentas

- `Python 3.10+`
- `Pandas`, `NumPy`, `Scikit-learn`, `XGBoost`
- `Matplotlib`, `Plotly`, `Seaborn`
- `Jupyter Notebooks`
- `ReportLab` ou `nbconvert` para geração de PDF
- `APIs públicas`: Tesouro Direto, Bacen, IBGE, etc.

---

## 📂 Estrutura do Projeto

