# 📊 Dashboard de Vendas Multi-Loja

**Análise completa de vendas com insights estratégicos e visualizações interativas**

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=flat&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat)

</div>

---

## 📌 Sobre o projeto

Análise de dados completa de vendas de múltiplas lojas, com geração de insights estratégicos e um dashboard visual para apoiar a tomada de decisão. Os dados foram extraídos de múltiplas planilhas Excel e integrados para uma visão unificada do negócio.

---

## 🎯 Objetivos

- ✅ Identificar as lojas com melhor e pior desempenho
- ✅ Analisar o faturamento total e por período
- ✅ Descobrir os produtos mais vendidos
- ✅ Avaliar a performance dos gerentes
- ✅ Comparar vendas gerais com o mês de dezembro
- ✅ Calcular o ticket médio por loja
- ✅ Criar visualizações gráficas dos indicadores

---

## 📈 Análises realizadas

| Métrica | Descrição |
|---------|-----------|
| **Faturamento Total** | Soma de todas as vendas do período |
| **Faturamento por Loja** | Ranking das lojas com melhor desempenho |
| **Faturamento por Gerente** | Performance individual dos gerentes |
| **Produtos Mais Vendidos** | Top produtos em quantidade vendida |
| **Ticket Médio** | Valor médio por venda em cada loja |
| **Análise Temporal** | Vendas por dia, mês, ano e dia da semana |

---

## 🛠️ Tecnologias utilizadas

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-11557C?style=flat)
![Seaborn](https://img.shields.io/badge/-Seaborn-4C72B0?style=flat)
![OpenPyXL](https://img.shields.io/badge/-OpenPyXL-217346?style=flat)

---

## 📂 Estrutura do projeto

```
dashboard-vendas/
│
├── estudo.ipynb              ← Notebook principal com toda a análise
├── requirements.txt          ← Dependências do projeto
├── README.md
├── .gitignore
│
└── planilha_estudo/          ← Pasta de dados (não incluída no repositório)
    ├── Vendas.xlsx           ← Dados gerais de vendas
    ├── Vendas - Dez.xlsx     ← Dados de dezembro
    └── Gerentes.xlsx         ← Dados dos gerentes
```

---

## 🚀 Como executar

### Passo 1 — Clone o repositório

```bash
git clone https://github.com/seu-usuario/dashboard-vendas.git
cd dashboard-vendas
```

### Passo 2 — Prepare os dados

> ⚠️ **Os arquivos de dados não estão incluídos no repositório por questões de privacidade.**

Crie a pasta `planilha_estudo/` na raiz do projeto e adicione os arquivos Excel com a estrutura abaixo:

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
jupyter notebook estudo.ipynb
```

> Ou abra pelo **VSCode** com a extensão Jupyter.

---

## 📊 Resultados e insights

Após executar a análise, você terá acesso a:

- **Faturamento Total** — visão geral do período completo
- **Ranking de Lojas** — identificação das melhores e piores lojas
- **Top Produtos** — produtos com maior volume de vendas
- **Ticket Médio** — valor médio por transação por loja
- **Sazonalidade** — análise de períodos de maior venda

### Visualizações geradas

| # | Gráfico |
|---|---------|
| 📊 | Barras do faturamento por loja |
| 📈 | Linha da evolução mensal das vendas |
| 📅 | Barras das vendas por dia da semana |
| 🥧 | Pizza da participação de dezembro |
| 🃏 | Cards com KPIs principais |

### Exemplo de saída

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
📈 Participação de Dezembro:   16.7%
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
&nbsp;·&nbsp;
[GitHub @TuusKBR](https://github.com/TuusKBR)
&nbsp;·&nbsp;
[LinkedIn](www.linkedin.com/in/abraão-dev)

)