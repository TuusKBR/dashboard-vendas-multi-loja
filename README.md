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
|---------|-----------|
| **Faturamento Total** | Soma de todas as vendas do período |
| **Top 10 Lojas** | Ranking das lojas com melhor desempenho |
| **Top 5 Piores Lojas** | Lojas com menor faturamento |
| **Faturamento por Gerente** | Performance individual dos gerentes |
| **Produtos Mais Vendidos** | Top 10 produtos em quantidade vendida |
| **Ticket Médio** | Valor médio por venda nas top 10 lojas |
| **Análise Temporal** | Vendas por mês, ano e dia da semana |
| **Participação de Dezembro** | Comparativo do mês de dezembro com o total |

---

## 🛠️ Tecnologias utilizadas

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/-Plotly-3F4F75?style=flat&logo=plotly&logoColor=white)
![OpenPyXL](https://img.shields.io/badge/-OpenPyXL-217346?style=flat)
![Jupyter](https://img.shields.io/badge/-Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

---

## 📂 Estrutura do projeto

```
dashboard-vendas-multi-loja/
│
├── notebooks/                    ← Notebooks com toda a análise
│   └── estudo.ipynb              ← Notebook principal
│
├── data/                         ← Pasta de dados (não incluída no repositório)
│   ├── Vendas.xlsx               ← Dados gerais de vendas
│   ├── Vendas - Dez.xlsx         ← Dados de dezembro
│   └── Gerentes.xlsx             ← Dados dos gerentes
│
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

---

## 🚀 Como executar

### Passo 1 — Clone o repositório

```bash
git clone https://github.com/TuusKBR/dashboard-vendas-multi-loja.git
cd dashboard-vendas-multi-loja
```

### Passo 2 — Prepare os dados

> ⚠️ **Os arquivos de dados não estão incluídos no repositório por questões de privacidade.**

Crie a pasta `data/` na raiz do projeto e adicione os arquivos Excel com a estrutura abaixo:

<details>
<summary><strong>Vendas.xlsx e Vendas - Dez.xlsx</strong></summary>

| Coluna | Tipo | Descrição |
|--------|------|-----------|
| `ID Loja` | int | Identificador da loja |
| `Data` | datetime | Data da venda |
| `Produto` | string | Nome do produto |
| `Quantidade` | int | Quantidade vendida |
| `Valor Final` | float | Valor total da venda |

</details>

<details>
<summary><strong>Gerentes.xlsx</strong></summary>

| Coluna | Tipo | Descrição |
|--------|------|-----------|
| `ID Loja` | int | Identificador da loja |
| `Gerente` | string | Nome do gerente |

</details>

### Passo 3 — Instale as dependências

```bash
pip install -r requirements.txt
```

### Passo 4 — Execute o notebook

```bash
jupyter notebook notebooks/estudo.ipynb
```

> Ou abra pelo **VSCode** com a extensão Jupyter.

---

## 📊 Visualizações geradas

| # | Gráfico | Descrição |
|---|---------|-----------|
| 📊 | Barras — Top 10 lojas | Faturamento das melhores lojas (escala verde) |
| 📉 | Barras — Top 5 piores | Lojas com menor faturamento (escala vermelha) |
| 📈 | Linha — Evolução mensal | Variação do faturamento ao longo dos meses |
| 👔 | Barras horizontais — Gerentes | Desempenho individual por gerente (escala verde) |
| 📦 | Barras — Produtos | Top 10 produtos mais vendidos em quantidade |
| 📅 | Barras — Dia da semana | Faturamento distribuído por dia (escala azul) |
| 📆 | Barras — Por ano | Comparativo anual (escala roxa) |
| 🃏 | Barras — Ticket médio | Top 10 lojas por valor médio de venda (escala teal) |

> Todos os gráficos possuem tema escuro (`#0d1117`), hover interativo personalizado e valores formatados em R$.

---

## 💡 Exemplo de saída

```
==================================================
              DESEMPENHO DAS LOJAS
==================================================
🥇 Melhor loja:  Loja A  —  R$ 150.000,00
🥉 Pior loja:    Loja B  —  R$  25.000,00
📊 Diferença:             R$ 125.000,00

==================================================
            COMPARAÇÃO COM DEZEMBRO
==================================================
💰 Vendas totais:              R$ 1.500.000,00
🎅 Vendas em Dezembro:         R$   250.000,00
📈 Participação de Dezembro:   16,7%
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
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Abraão_Dev-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/abraão-dev)