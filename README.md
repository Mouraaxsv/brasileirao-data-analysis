# ⚽ Brasileirão Data Analysis

Análise exploratória, limpeza e engenharia de atributos de uma base histórica de partidas do Campeonato Brasileiro Série A, preparando os dados para futuras visualizações, dashboards e modelos de Machine Learning.

---

## 📋 Sobre a base

Partidas do Brasileirão Série A desde **2003**, incluindo:

- Estádio, árbitro, público e técnicos
- Colocação, valor e idade média dos elencos titulares
- Gols de cada partida
- Estatísticas detalhadas de jogo a partir de **2018** (escanteios, faltas, chutes, defesas, impedimentos)

## 🎯 Progresso do projeto

- [x] Limpeza e tratamento dos dados
- [ ] Visualização de estatísticas
- [ ] Construção de dashboard
- [ ] Aplicação de Machine Learning

## 🚀 Como executar

**1.** Clone o repositório e entre na pasta do projeto.

**2.** Crie e ative um ambiente virtual:

```bash
python -m venv .venv

.venv\Scripts\activate      # Windows
source .venv/bin/activate   # Linux/macOS
```

**3.** Instale as dependências:

```bash
pip install -r requirements.txt
```

**4.** Abra o notebook:

```bash
jupyter lab notebooks/EDA.ipynb
```

> ⚠️ O notebook lê os dados de `data/raw/brasileirao.csv` usando caminho relativo, portanto **deve ser executado a partir da pasta `notebooks/`**. A base tratada é salva em `data/processed/brasileirao_clean.csv`.

## 📓 Notebook: `EDA.ipynb`

| # | Seção | Conteúdo |
|---|-------|----------|
| 1 | **Carregamento dos Dados** | Leitura do CSV e inspeção inicial (`shape`, `columns`, `info`) |
| 2 | **Exploração Inicial** | Estatísticas descritivas, contagem de valores ausentes e observações sobre a base |
| 3 | **Limpeza dos Dados** | Conversão de tipos, verificação de duplicatas e tratamento de valores ausentes |
| 4 | **Engenharia de Atributos** | Colunas de data (`ano`, `mes`, `dia`), validações de consistência, padronização de texto, criação de `total_gols` e `resultado` |
| 5 | **Exportação da Base Tratada** | Geração de `data/processed/brasileirao_clean.csv` |
| 6 | **Conclusão** | Resumo das decisões tomadas e próximos passos |

## 📂 Estrutura do projeto

```
brasileirao-data-analysis/
├── data/
│   ├── raw/                  # Dados originais, não tratados
│   │   └── brasileirao.csv
│   └── processed/            # Dados tratados, gerados pelo notebook
│       └── brasileirao_clean.csv
├── notebooks/
│   └── EDA.ipynb             # Análise exploratória, limpeza e engenharia de atributos
├── requirements.txt
└── LICENSE
```

## 🛠️ Tecnologias

`Python` · `Pandas` / `NumPy` · `Matplotlib` / `Seaborn` / `Plotly` · `Scikit-Learn` · `Jupyter Notebook`

## 📄 Licença

Este projeto está sob a licença [MIT](LICENSE).
