# 📊 Simulador de Investimento em Projetos

Este documento apresenta a estrutura e as análises financeiras para avaliação de viabilidade de projetos de investimento.

---

## 📌 1. Visão Geral do Projeto

| Parâmetro | Valor / Descrição |
| :--- | :--- |
| **Nome do Projeto** | Projeto Etega |
| **Investimento Inicial ($I_0$)** | R$ 100.000,00 |
| **Taxa Mínima de Atratividade (TMA)** | 10% a.a. |
| **Horizonte de Análise** | 5 anos |

---

## 📈 2. Fluxo de Caixa Projetado

A tabela abaixo detalha os fluxos de caixa operacionais e acumulados ao longo do horizonte do projeto:

| Ano ($t$) | Investimento / Reinvestimento | Receitas Operacionais | Custos Operacionais | Fluxo de Caixa Líquido ($FC_t$) | Fluxo de Caixa Acumulado |
| :---: | :---: | :---: | :---: | :---: | :---: |
| **0** | R$ (100.000,00) | R$ 0,00 | R$ 0,00 | **R$ (100.000,00)** | R$ (100.000,00) |
| **1** | R$ 0,00 | R$ 50.000,00 | R$ 20.000,00 | **R$ 30.000,00** | R$ (70.000,00) |
| **2** | R$ 0,00 | R$ 60.000,00 | R$ 22.000,00 | **R$ 38.000,00** | R$ (32.000,00) |
| **3** | R$ 0,00 | R$ 70.000,00 | R$ 25.000,00 | **R$ 45.000,00** | R$ 13.000,00 |
| **4** | R$ 0,00 | R$ 75.000,00 | R$ 27.000,00 | **R$ 48.000,00** | R$ 61.000,00 |
| **5** | R$ 0,00 | R$ 80.000,00 | R$ 30.000,00 | **R$ 50.000,00** | R$ 111.000,00 |

---

## 🧮 3. Indicadores Financeiros de Viabilidade

### 📐 Fórmulas Utilizadas

1. **Valor Presente Líquido (VPL):**
   $$VPL = \sum_{t=1}^{n} \frac{FC_t}{(1 + i)^t} - I_0$$

2. **Taxa Interna de Retorno (TIR):**
   $$\sum_{t=0}^{n} \frac{FC_t}{(1 + TIR)^t} = 0$$

3. **Índice de Lucratividade (IL):**
   $$IL = \frac{\sum_{t=1}^{n} \frac{FC_t}{(1 + i)^t}}{I_0}$$

---

### 📊 Resumo dos Resultados

| Indicador | Sigla | Valor Apurado | Crivo / Regra de Decisão | Status |
| :--- | :---: | :---: | :--- | :---: |
| **Valor Presente Líquido** | `VPL` | R$ 57.181,92 | $VPL > 0$ | 🟢 Viável |
| **Taxa Interna de Retorno** | `TIR` | 28,34% | $TIR > TMA$ (10%) | 🟢 Viável |
| **Payback Simples** | `PB` | 2,71 anos (~ 2 anos e 8 meses) | Menor que o horizonte estipulado | 🟢 Adequado |
| **Payback Descontado** | `PBD` | 3,24 anos (~ 3 anos e 3 meses) | Menor que o horizonte estipulado | 🟢 Adequado |
| **Índice de Lucratividade** | `IL` | 1,57 | $IL > 1,0$ | 🟢 Atrativo |

---

## 📝 4. Conclusão e Recomendação

 Com base na análise dos indicadores econômico-financeiros:
- O **VPL positivo** indica geração de valor acima do custo de oportunidade estipulado (TMA de 10%).
- A **TIR de 28,34%** supera significativamente a taxa mínima exigida.
- O investimento inicial é recuperado em termos descontados em aproximadamente **3 anos e 3 meses**.

**Recomendação:** O projeto apresenta forte viabilidade financeira e é recomendado para aprovação e execução.