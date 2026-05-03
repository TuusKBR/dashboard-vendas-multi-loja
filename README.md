# 📊 Dashboard de Vendas Multi-Loja

**Análise completa de vendas com insights estratégicos e visualizações interativas**

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=flat&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-5.0+-3F4F75?style=flat&logo=plotly&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat)

---

## 📌 Sobre o projeto

Análise de dados completa de vendas de múltiplas lojas, com geração de insights estratégicos e um dashboard visual interativo para apoiar a tomada de decisão. Os dados foram extraídos de múltiplas planilhas Excel e integrados para uma visão unificada do negócio.

Todos os gráficos foram construídos com **Plotly Express**, garantindo interatividade com hover personalizado, paletas de cores temáticas e layout escuro profissional.

---

## 🎯 Objetivos

- ✅ Identificar as lojas com melhor e pior desempenho
- ✅ Analisar o faturamento total e por período
- ✅ Descobrir os produtos mais vendidos
- ✅ Avaliar a performance dos gerentes
- ✅ Comparar vendas gerais com o mês de dezembro
- ✅ Calcular o ticket médio por loja
- ✅ Criar visualizações gráficas interativas dos indicadores

---

## 📈 Análises realizadas

| Métrica | Descrição |
|---|---|
| **Faturamento Total** | Soma de todas as vendas do período |
| **Top 10 Lojas** | Ranking das lojas com melhor desempenho |
| **Top 5 Piores Lojas** | Lojas com menor faturamento |
| **Faturamento por Gerente** | Performance individual dos gerentes |
| **Produtos Mais Vendidos** | Top 10 produtos em quantidade vendida |
| **Ticket Médio** | Valor médio por venda nas top 10 lojas |
| **Análise Temporal** | Vendas por mês, ano e dia da semana |

---

## 🛠️ Tecnologias utilizadas

| Tecnologia | Finalidade |
|---|---|
| **Python** | Linguagem principal |
| **Pandas** | Manipulação e tratamento dos dados |
| **Plotly Express** | Criação de gráficos interativos |
| **OpenPyXL** | Leitura de arquivos Excel |
| **Jupyter Notebook** | Ambiente de desenvolvimento e análise |

---

## 📂 Estrutura do projeto

```
dashboard-vendas-multi-loja/
│
├── data/                        ← Dados do projeto
│   └── planilha_vendas/         ← Planilhas Excel
│       ├── Vendas.xlsx          ← Dados gerais de vendas
│       ├── Vendas - Dez.xlsx    ← Dados de dezembro
│       └── Gerentes.xlsx        ← Dados dos gerentes
│
├── notebooks/                   ← Notebooks com as análises
│   └── analise.ipynb            ← Notebook principal
│
├── .venv/                       ← Ambiente virtual
├── .gitignore                   ← Arquivos ignorados pelo Git
├── LICENSE                      ← Licença do projeto
├── README.md                    ← Documentação
└── requirements.txt             ← Dependências do projeto
```

---

## 🚀 Como executar

### Passo 1 — Clone o repositório

```bash
git clone https://github.com/TuusKBR/dashboard-vendas-multi-loja.git
cd dashboard-vendas-multi-loja
```

### Passo 2 — Crie o ambiente virtual

```bash
python -m venv .venv
```

Ative o ambiente virtual:

- **Windows:** `.venv\Scripts\activate`
- **Linux/Mac:** `source .venv/bin/activate`

### Passo 3 — Instale as dependências

```bash
pip install -r requirements.txt
```

### Passo 4 — Execute o Jupyter Notebook

```bash
jupyter notebook
```

No navegador que abrir, navegue até a pasta `notebooks/` e abra o arquivo `analise.ipynb`.

> 💡 **Dica:** Você também pode abrir diretamente com o VSCode (extensão Jupyter) ou executar célula por célula no navegador.

---

## 📊 Visualizações geradas

| # | Gráfico | Descrição |
|---|---|---|
| 📊 | Barras — Top 10 lojas | Faturamento das melhores lojas (escala verde) |
| 📉 | Barras — Top 5 piores | Lojas com menor faturamento (escala vermelha) |
| 📈 | Linha — Evolução mensal | Variação do faturamento ao longo dos meses |
| 👔 | Barras horizontais — Gerentes | Desempenho individual por gerente |
| 📦 | Barras — Produtos | Top 10 produtos mais vendidos em quantidade |
| 📅 | Barras — Dia da semana | Faturamento distribuído por dia (escala azul) |
| 📆 | Barras — Por ano | Comparativo anual (escala roxa) |
| 💰 | Barras — Ticket médio | Top 10 lojas por valor médio de venda (escala teal) |

> Todos os gráficos possuem tema escuro (`#0d1117`), hover interativo personalizado e valores formatados em R$ (Real brasileiro).

---

## 📋 Estrutura dos dados

### `Vendas.xlsx` e `Vendas - Dez.xlsx`

| Coluna | Tipo | Descrição |
|---|---|---|
| `ID Loja` | int | Identificador da loja |
| `Data` | datetime | Data da venda |
| `Produto` | string | Nome do produto |
| `Quantidade` | int | Quantidade vendida |
| `Valor Final` | float | Valor total da venda |

### `Gerentes.xlsx`

| Coluna | Tipo | Descrição |
|---|---|---|
| `ID Loja` | int | Identificador da loja |
| `Gerente` | string | Nome do gerente |

---

## 🔧 Personalização

### Alterar cores dos gráficos

No notebook `analise.ipynb`, localize as configurações de cores:

```python
# Exemplo: mudar a cor do gráfico de evolução mensal
fig2.update_traces(
    line=dict(color='#SUA_COR', width=3),
    marker=dict(size=8, color='#OUTRA_COR')
)
```

### Alterar tema padrão

```python
import plotly.io as pio
pio.templates.default = "plotly_dark"  # ou "plotly_white", "ggplot2", etc.
```

---

## 📝 Fluxo de análise

O notebook `analise.ipynb` está organizado nas seguintes seções:

1. **Importação de bibliotecas** — Importa pandas, plotly e outras dependências
2. **Carregamento dos dados** — Leitura dos arquivos Excel
3. **Tratamento dos dados** — Limpeza, conversões e criação de colunas auxiliares
4. **Métricas principais** — Cálculo de KPIs como faturamento e ticket médio
5. **Análise por loja** — Ranking das melhores e piores lojas
6. **Evolução mensal** — Tendência do faturamento ao longo do tempo
7. **Análise por gerente** — Performance individual dos gerentes
8. **Produtos mais vendidos** — Ranking de produtos por quantidade
9. **Faturamento por dia da semana** — Padrões de compra por dia
10. **Faturamento por ano** — Comparativo anual
11. **Ticket médio por loja** — Valor médio gasto por venda

---

## 💡 Exemplo de saída

```
==================================================
              DESEMPENHO DAS LOJAS
==================================================
🥇 Melhor loja:  Loja A  —  R$ 150.000,00
🥉 Pior loja:    Loja B  —  R$  25.000,00
📊 Diferença:             R$ 125.000,00
```

---

## 🤝 Contribuição

Contribuições são bem-vindas! Siga os passos:

1. Faça um **Fork** do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'feat: adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um **Pull Request**

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 👨‍💻 Autor

**Abraão Rubens**

[![GitHub](https://img.shields.io/badge/GitHub-@TuusKBR-181717?style=flat&logo=github)](https://github.com/TuusKBR)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Abraão_Dev-0A66C2?style=flat&logo=linkedin)](https://linkedin.com/in/abraao-dev)