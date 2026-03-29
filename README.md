# Estudo de Correlação e Causalidade entre Produtos Complementares

> **Existe relação entre as vendas de dois produtos? E se um crescer, o outro também cresce?**  
> Esse estudo responde essas perguntas com estatística aplicada a dados de vendas mensais.

---

## Contexto e Objetivo

Em contextos de negócio, é comum suspeitar que o desempenho de um produto influencia o de outro — mas suspeita não é evidência.

Este estudo investiga, com base em dados de vendas mensais, se as vendas do **Produto A** e do **Produto B** são correlacionadas e se uma variável é capaz de **prever** o comportamento da outra ao longo do tempo.

A base de dados utilizada é fictícia, construída para preservar os padrões estatísticos de um estudo real: tendência de crescimento, sazonalidade e correlação positiva entre os produtos.

---

## Técnicas Utilizadas

| Técnica | Objetivo |
|---|---|
| **Análise Exploratória (EDA)** | Validar e entender a base antes de qualquer análise |
| **Detecção de Outliers (IQR)** | Remover meses atípicos que distorceriam a correlação |
| **Correlação de Pearson** | Medir a força e direção da relação linear entre os produtos |
| **Regressão Linear Simples** | Quantificar o quanto B responde a variações em A |
| **Teste de Causalidade de Granger** | Verificar se o histórico de A ajuda a prever o futuro de B (e vice-versa) |

---

## Principais Resultados

- Correlação de Pearson **forte e positiva** entre os dois produtos
- Regressão Linear com **R² > 0.80** — B responde de forma previsível a A
- Teste de Granger confirmou **causalidade bidirecional** nos lags de 1 a 3 meses
- Os produtos se influenciam mutuamente, sugerindo uma **dinâmica complementar**

---

## Quando Aplicar esse Tipo de Estudo?

Esse tipo de análise é útil sempre que houver a dúvida:  
*"será que o desempenho de X influencia o desempenho de Y?"*

Exemplos práticos:

- **Vendas:** as vendas de um produto de entrada preveem as de um produto premium?
- **Marketing:** o investimento em mídia paga influencia as buscas orgânicas?
- **Operações:** o volume de pedidos de um canal antecipa o de outro canal?
- **Financeiro:** a variação de um indicador econômico influencia a receita da empresa?
- **Produto:** o engajamento com uma feature do app antecipa a adoção de outra?

---

## Estrutura do Repositório

```
📦 estudo-correlacao-produtos/
├── 📓 estudo_correlacao_produto_a_vs_b.ipynb   # Notebook principal
└── 📄 README.md                                 # Este arquivo
```

---

## Como Rodar

1. Clone o repositório ou baixe o `.ipynb`
2. Instale as dependências:
```bash
pip install pandas numpy matplotlib scikit-learn scipy statsmodels
```
3. Abra o notebook no Jupyter e execute **Kernel → Restart & Run All**

> Os dados já estão embutidos no notebook — não é necessário nenhum arquivo externo.

---

## Autora

**Ana Paula Martini**  
[LinkedIn](https://www.linkedin.com/in/ana-paula-martini-ba886961/)
