# Análise de Delivery de Refeições (Pandas + NumPy)

Desafio prático da Rocketseat: análise de pedidos de um delivery de refeições, do tratamento dos dados ao cálculo de KPIs.

## O que foi feito

1. Análise exploratória (`head`, `tail`, `info`, `describe`)
2. Criação da coluna `Receita_Item` (quantidade × preço unitário)
3. Tratamento de nulos (média em `Quantidade`; remoção de linhas sem `Preco_Unitario`)
4. Agregações por item e top 5 (por quantidade e por receita)
5. Análise temporal (receita por mês e evolução por ano-mês)
6. Merge com o cardápio e receita por categoria
7. Filtro: Salgados com mais de 10 unidades
8. KPIs com NumPy (receita total, itens vendidos, ticket médio) e percentis

## Principais resultados

| Indicador | Valor |
|---|---|
| Receita total | R$ 122.652,59 |
| Itens vendidos | 6.833 |
| Ticket médio | R$ 285,24 |
| Categoria líder | Salgados (~43% da receita) |
| Item mais vendido | Hamburguer |
| Item com maior receita | Pizza Calabresa |

## Estrutura

```
.
├── dados/
│   ├── pedidos.csv
│   └── cardapio.csv
├── desafio_delivery.ipynb
└── README.md
```

## Como executar

```bash
pip install pandas numpy matplotlib jupyter
jupyter notebook desafio_delivery.ipynb
```

Também funciona no Google Colab: envie os CSVs (dentro de `dados/` ou na mesma pasta do notebook) e execute as células em ordem.

O notebook procura os arquivos em `dados/` e, se a pasta não existir, na pasta atual.
