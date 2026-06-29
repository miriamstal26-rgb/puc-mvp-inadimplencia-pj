# 📊 Previsão de Inadimplência com Regressão Ridge

## 📌 Descrição
Este projeto tem como objetivo prever a taxa de inadimplência utilizando variáveis macroeconômicas e um modelo de regressão linear regularizada (Ridge).

A análise foi desenvolvida com foco em capturar padrões temporais e avaliar a capacidade preditiva do modelo em relação a um baseline simples.

---

## 🎯 Objetivo
- Modelar a inadimplência ao longo do tempo
- Avaliar o desempenho de um modelo Ridge
- Comparar os resultados com um baseline
- Identificar limitações e oportunidades de melhoria

---

## 📊 Dados
- Série temporal mensal de inadimplência
- Variáveis macroeconômicas com defasagem (lag)
- Período: 04/2023 a 01/2026

---

## ⚙️ Modelo
- Tipo: Ridge Regression
- Alpha: 1.0
- Features com lag de 3 meses

---

## 📈 Resultados

| Modelo          | MAE    | RMSE   | R²     |
|-----------------|--------|--------|--------|
| Baseline        | 1.9017 | 2.7479 | -0.4903|
| Ridge (alpha=1) | 1.2104 | 1.5211 |  0.5434|

---

## 📉 Análise

### Real vs Previsto
O modelo acompanha bem a tendência, com melhor desempenho a partir de 2025.  
Há subestimação no início (2023–2024), possivelmente devido ao lag das variáveis.

### Resíduos
- Distribuição aleatória (bom sinal)
- Maiores erros entre 15% e 18%

---

## ⚠️ Limitações
- Série curta
- Lag fixo de 3 meses
- Falta de variáveis (desemprego, PIB, etc.)
- Não captura quebras estruturais

---

## 🚀 Melhorias Futuras
- Testar múltiplos lags
- Incluir novas variáveis
- Testar modelos mais complexos

---

## 📌 Conclusão
O modelo Ridge superou o baseline e capturou padrões relevantes.

---

##  Autora
Miriam Stal
