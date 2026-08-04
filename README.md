# 📊 Pipeline de Vendas — Do CSV ao Dashboard

Pipeline de dados end-to-end para análise de vendas: ingestão de arquivos CSV brutos, tratamento em Python e entrega de um dashboard interativo em Power BI com visão de faturamento, ticket médio, margem e ranking de produtos.

> ⚠️ **Dados fictícios**, utilizados apenas para fins de demonstração técnica.

---

## 🎯 Objetivo

Transformar bases de vendas brutas e dispersas em um modelo analítico confiável, permitindo à gestão comparar desempenho mês a mês e identificar produtos e regiões de maior impacto — sem depender de planilhas manuais.

---

## 🧱 Arquitetura do pipeline

```
CSV bruto (vendas)
      │
      ▼
[1] Extração dos arquivos brutos
      │
      ▼
[2] Limpeza e padronização (Python / pandas)
      │
      ▼
[3] Modelagem em estrela (fato vendas + dimensões)
      │
      ▼
[4] Medidas DAX (receita, ticket médio, margem)
      │
      ▼
[5] Dashboard interativo (Power BI) — por região e período
```

### Etapas detalhadas

**1. Extração**
Leitura dos arquivos CSV de origem contendo os registros brutos de vendas (pedidos, itens, valores, datas, região).

**2. Limpeza e padronização (Python / pandas)**
- Tratamento de valores nulos e duplicados
- Padronização de tipos (datas, moedas, categorias)
- Validação de consistência entre arquivos

**3. Modelagem em estrela**
- Tabela fato: `fato_vendas`
- Tabelas dimensão: `dim_produto`, `dim_cliente`, `dim_regiao`, `dim_calendario`
- Relacionamentos otimizados para performance no Power BI

**4. Medidas DAX**
- Receita total e por período
- Ticket médio
- Margem (%) por produto/categoria
- Variação mês a mês (MoM)

**5. Dashboard**
Painel interativo com filtros por região e período, ranking de produtos e comparativo de faturamento.

---

## 📈 Resultados

- Consolidação de **[X]** mil linhas de dados brutos em um modelo único
- Visão única de faturamento com comparativo mês a mês
- Redução do tempo de análise manual em planilhas de **[X]** para poucos minutos de refresh

*(Substituir os campos `[X]` pelos números reais do projeto.)*

---

## 🛠️ Tecnologias utilizadas

| Categoria | Ferramentas |
|---|---|
| Linguagem | Python (pandas) |
| Consulta/Modelagem | SQL |
| Visualização | Power BI, DAX |
| Versionamento | Git / GitHub |

---

## 📂 Estrutura do repositório

```
pipeline-vendas/
├── data/               # dados brutos e tratados (ou amostra fictícia)
├── notebooks/          # exploração e tratamento em Python
├── src/                # scripts de ETL
├── dashboard/          # arquivo .pbix do Power BI
├── images/             # prints do dashboard
└── README.md
```

---

## ▶️ Como executar

```bash
# Clonar o repositório
git clone https://github.com/lui5henrique/NOME-DO-REPO.git
cd NOME-DO-REPO

# Instalar dependências
pip install -r requirements.txt

# Executar o pipeline de tratamento
python src/etl.py
```

O arquivo `dashboard/pipeline-vendas.pbix` pode ser aberto diretamente no Power BI Desktop.

---

## 🖼️ Prévia do dashboard

*(Inserir aqui um print ou GIF do painel final)*

---

## 👤 Autor

**Luis Henrique** — Analista de Dados e BI
[Portfólio](https://luishenrique-analyticsdata.lovable.app/) · [LinkedIn](#) · [GitHub](https://github.com/lui5henrique)
