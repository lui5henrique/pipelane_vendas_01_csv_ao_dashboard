<h1 align="center">Painel de Vendas — Gestão de Loja</h1>

<p align="center">Dashboard interativo de vendas em uma única página HTML, com filtros, KPIs e gráficos</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-orange" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-blue" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-yellow" alt="JavaScript">
  <img src="https://img.shields.io/badge/Chart.js-4.4.1-informational" alt="Chart.js">
</p>

> ⚠️ **Dados fictícios**, utilizados apenas para fins de demonstração técnica.

## Sobre o projeto

Dashboard de gestão de vendas de uma loja de artigos esportivos, entregue como um único arquivo HTML — sem backend, sem build, sem dependências além de uma biblioteca de gráficos carregada via CDN. Os dados (100 vendas fictícias de 2025, com produto, categoria, marca, região, cliente e valores) ficam embutidos diretamente no próprio arquivo.

<img width="1877" height="851" alt="Captura de tela 2026-09-06 101730" src="https://github.com/user-attachments/assets/9d0b9dbe-48d4-470d-bd37-69987337675d" />
<img width="1882" height="846" alt="Captura de tela 2026-09-06 101859" src="https://github.com/user-attachments/assets/d1403598-32ed-4722-86d7-cd68bbd5f154" />


## Funcionalidades

- KPIs: faturamento total, lucro total, margem de lucro (%), ticket médio, custo total e quantidade vendida.
- Filtros por categoria, produto, região e marca, com tags removíveis para os filtros ativos.
- Gráficos (Chart.js): faturamento e lucro por mês, vendas por canal, vendas por região, margem por categoria e perfil por faixa etária.
- Tabelas de Top 5 Produtos (por margem), Top 5 Clientes e Produtos com Menor Margem.

## Tecnologias

- HTML5 / CSS3 / JavaScript (vanilla, sem framework)
- [Chart.js](https://www.chartjs.org/) (via CDN) — gráficos

## Como executar

Por ser um único arquivo estático, basta abrir direto no navegador:

```bash
git clone https://github.com/lui5henrique/pipelane_vendas_01_csv_ao_dashboard.git
cd pipelane_vendas_01_csv_ao_dashboard
```

Depois é só abrir o `index.html` (duplo clique ou arrastar para o navegador). Não é necessário servidor local, pois os dados já estão embutidos no arquivo — não há `fetch` de arquivos externos.

## Estrutura do projeto

```
index.html    dashboard completo: estrutura, estilo e dados/JS embutidos no mesmo arquivo
```

## Autor

**Luis Henrique** — [@lui5henrique](https://github.com/lui5henrique)
