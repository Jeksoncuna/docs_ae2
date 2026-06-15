# 🌱 SP Verde & Ar — Qualidade do Ar e Arborização Urbana em São Paulo

Projeto extensionista com dados que analisa a distribuição da **arborização urbana** e da **qualidade do ar** nos 96 distritos de São Paulo, identificando desigualdades territoriais e vulnerabilidade socioambiental.

> Disciplina: Projeto Integrador extensionista | São Paulo, SP | 2026

---

## 🎯 Objetivo

Construir indicadores de cobertura arbórea (ICA), exposição à poluição (IEP) e vulnerabilidade socioambiental (IVSA) por distrito, gerando um dashboard e dataset aberto para uso público.

---

## ❓ Perguntas Analíticas

| # | Pergunta |
|---|----------|
| PA1 | Quais distritos têm menor arborização e pior qualidade do ar simultaneamente? |
| PA2 | Existe correlação entre IDH distrital e cobertura arbórea? |
| PA3 | Como o PM2,5 varia entre período seco e chuvoso? |
| PA4 | Qual proporção da população de baixa renda está exposta a PM2,5 acima do limite da OMS? |

---

## 🗃️ Fontes de Dados

| Fonte | Dados | Acesso |
|-------|-------|--------|
| GeoSampa (PMSP) | Cobertura vegetal por distrito | geosampa.prefeitura.sp.gov.br |
| CETESB | PM2,5, PM10, O3 por estação | cetesb.sp.gov.br/ar |
| IBGE — Censo 2022 | Renda per capita e IDH | sidra.ibge.gov.br |
| InfoSiga SP | Internações respiratórias | infosiga.sp.gov.br |

---

## 🗂️ Estrutura do Repositório

```
projeto-sp-verde-ar/
├── docs/escopo-1/
│   ├── AE1/   ← Termo de Abertura + Plano do Projeto
│   └── AE2/   ← Dicionário de Dados, Modelo Lógico, Wireframe
├── data/
│   ├── raw/         ← dados brutos
│   ├── processed/   ← dados limpos
│   └── quality_reports/
├── notebooks/       ← EDA, análise espacial, cálculo IVSA
├── src/             ← coleta.py, limpeza.py, qualidade.py
├── dashboard/       ← app.py (Plotly Dash)
└── .gitignore
```

---

## 🚀 Como Executar

```bash
pip install pandas geopandas plotly dash folium scipy
jupyter notebook notebooks/
# Dashboard: cd dashboard && python app.py
```

---

## 📁 Documentação

- [AE1 — Termo de Abertura](./docs/escopo-1/AE1/AE1_Projeto_Extensionista.docx)
- [AE2 — Desenho da Solução](./docs/escopo-1/AE2/AE2_Desenho_Solucao.pdf)

---

## 🔒 Ética e LGPD

Apenas dados públicos e agregados por distrito. Base legal: Art. 7º, II da LGPD. Licença: MIT.
