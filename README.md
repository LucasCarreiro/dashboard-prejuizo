# Dashboard de prejuízo

Página única em HTML + JavaScript que lê uma planilha de vendas (.xlsx) **no próprio navegador** e mostra onde a operação está perdendo dinheiro:

- Top 5 categorias por prejuízo
- Filiais com maiores prejuízos
- Top 10 produtos por prejuízo
- Resumo geral: total de vendas e total de prejuízo

**[Abrir o dashboard](https://lucascarreiro.github.io/dashboard-prejuizo/)** e importar a planilha de exemplo [`exemplo-vendas.xlsx`](exemplo-vendas.xlsx), que tem dados fictícios.

> O arquivo é lido localmente com SheetJS. Nada é enviado para servidor nenhum.

## Formato da planilha

A **primeira aba** precisa ter uma linha de cabeçalho e, a partir da segunda linha, um registro por produto e filial. O painel usa estas colunas:

| Coluna | Conteúdo |
|---|---|
| A | Filial |
| E | Categoria |
| G | Produto |
| I | Venda (R$) |
| P | Resultado (R$): valores negativos indicam prejuízo |

As demais colunas (data, código, custo, margem, etc.) podem existir normalmente. O arquivo também precisa de uma **segunda aba**, reservada às metas de margem.

## Tecnologias

HTML · JavaScript · [Chart.js](https://www.chartjs.org/) · [SheetJS](https://sheetjs.com/)

---

Feito por **Lucas Carreiro** · [LinkedIn](https://www.linkedin.com/in/lucas1carreiro1/)
