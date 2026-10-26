# ML-00-Fundamentos-estatistica-probabilidade

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23669967.svg)](https://doi.org/10.5281/zenodo.23669967)
[![Licença: CC BY-NC-SA 4.0](https://img.shields.io/badge/licen%C3%A7a-CC%20BY--NC--SA%204.0-lightgrey.svg)](LICENSE)

Uma **introdução prática e didática à estatística e à probabilidade para Machine Learning**, usando Python.

📖 **Leia como livro interativo:** https://joaobleite.github.io/ML-00-Fundamentos-estatistica-probabilidade/

Este é o livro de **nivelamento** de uma série de estudos. Ele vem **antes** de:
- [ML-01-Introducao-regressao](https://github.com/JoaoBLeite/ML-01-Introducao-regressao), que ensina **regressão** (prever um número);
- [ML-02-Introducao-classificacao](https://github.com/JoaoBLeite/ML-02-Introducao-classificacao), que ensina **classificação** (prever uma categoria).

## 🎯 Objetivo

Os livros de ML usam o tempo todo palavras como *média*, *desvio padrão*, *correlação*, *probabilidade*, *distribuição*, *intervalo de confiança*, *verossimilhança* e *log loss*. Este repositório constrói cada uma delas do zero, para quem está **começando em Machine Learning e em Python**, ao longo de 16 notebooks e mais dois extras.

O foco é **entender o porquê**, não decorar fórmulas:

- 🎓 **Cada conceito novo** é apresentado e contextualizado antes de ser usado, com uma analogia do dia a dia.
- 🎲 **Simular antes de formular**: sempre que possível, a ideia aparece primeiro numa simulação com o computador, e só depois a fórmula, conferindo que as duas batem.
- 💬 **Cada célula de código** tem comentários explicando tanto a ideia estatística quanto a sintaxe Python.
- 📌 **Cada análise termina com uma conclusão**: o que os números e gráficos estão dizendo.
- 🔗 **Pontes para o ML**: cada conceito mostra onde ele reaparece no ML-01 e no ML-02.

### Os dados

Para não competir com os datasets dos outros livros, usamos dados **pequenos e conhecidos**, além de muitos dados **simulados**:

- **tips** (gorjetas): 244 mesas atendidas por um garçom num restaurante dos EUA, com o valor da conta, a gorjeta, o dia, a refeição, o tamanho da mesa e se havia fumantes.
- **penguins** (pinguins): medidas do corpo de 344 pinguins de três espécies da Antártida (Adelie, Chinstrap e Gentoo), de três ilhas.
- **Dados simulados** com o numpy, em que conhecemos a "resposta verdadeira" e podemos medir o erro de cada método.

## 📚 Trilha de estudos

### Parte I · Estatística descritiva

| Notebook | O que você aprende |
|---|---|
| [01 · Dados e tipos de variáveis](01_dados_e_tipos_de_variaveis.ipynb) | População × amostra, tipos de variáveis, primeiros passos com numpy e pandas, frequências, faixas e valores ausentes |
| [02 · Medidas de tendência e dispersão](02_medidas_de_tendencia_e_dispersao.ipynb) | Média, mediana e moda, outliers, variância e desvio padrão, o $n-1$ (correção de Bessel), quantis e IQR, assimetria e curtose, e por que a média combina com o MSE e a mediana com o MAE |
| [03 · Visualizando distribuições](03_visualizando_distribuicoes.ipynb) | Histograma, KDE, boxplot, violino, ECDF, distribuições bimodais e a transformação logarítmica |
| [04 · Relações entre variáveis](04_relacoes_entre_variaveis.ipynb) | Covariância, correlação de Pearson e de Spearman, quarteto de Anscombe, tabelas de contingência, correlação ≠ causalidade e o paradoxo de Simpson |

### Parte II · Probabilidade

| Notebook | O que você aprende |
|---|---|
| [05 · Fundamentos de probabilidade](05_fundamentos_de_probabilidade.ipynb) | Espaço amostral e eventos, probabilidade por simulação, axiomas, regras do complemento e da união, contagem, o problema do aniversário e o de Monty Hall |
| [06 · Probabilidade condicional e Bayes](06_probabilidade_condicional_e_bayes.ipynb) | Probabilidade condicional, independência, probabilidade total, Teorema de Bayes, a armadilha da taxa base e um Naive Bayes à mão |
| [07 · Variáveis aleatórias discretas](07_variaveis_aleatorias_discretas.ipynb) | PMF, valor esperado e variância, distribuições Bernoulli, binomial, Poisson e geométrica, e a incerteza da acurácia num teste pequeno |
| [08 · Variáveis aleatórias contínuas](08_variaveis_aleatorias_continuas.ipynb) | Densidade e CDF, distribuições uniforme, normal, exponencial e log-normal, z-score, Q-Q plot e ajuste de distribuições |
| [09 · Distribuições conjuntas](09_distribuicoes_conjuntas.ipynb) | Distribuições conjunta, marginal e condicional, esperança condicional, normal multivariada, matriz de covariância, direções principais (PCA) e distância de Mahalanobis |

### Parte III · Inferência estatística

| Notebook | O que você aprende |
|---|---|
| [10 · Lei dos Grandes Números e TCL](10_lei_dos_grandes_numeros_e_tcl.ipynb) | LGN (e a Cauchy, em que ela falha), distribuição amostral, erro padrão $\sigma/\sqrt{n}$, Teorema Central do Limite e aproximação normal da binomial |
| [11 · Estimação e intervalos de confiança](11_estimacao_e_intervalos_de_confianca.ipynb) | Viés, variância e EQM de um estimador, troca entre viés e variância, distribuição t, intervalos de confiança, ICs para proporções e bootstrap |
| [12 · Testes de hipótese](12_testes_de_hipotese.ipynb) | p-valor, teste de permutação, teste t, qui-quadrado, erros tipo I e II, poder, teste pareado para comparar modelos, testes múltiplos e significância × importância prática |
| [13 · Máxima verossimilhança](13_maxima_verossimilhanca.ipynb) | Verossimilhança e log-verossimilhança, EMV por fórmula e por otimização, por que a regressão linear usa o MSE e a logística usa a log loss, e o AIC |

### Parte IV · Ponte para o ML

| Notebook | O que você aprende |
|---|---|
| [14 · Regressão linear estatística](14_regressao_linear_estatistica.ipynb) | A tabela do statsmodels, erros padrão e ICs dos coeficientes, regressão múltipla, intervalo de previsão, análise de resíduos, erros padrão robustos e VIF |
| [15 · Entropia e informação](15_entropia_e_informacao.ipynb) | Entropia, entropia cruzada (a log loss), divergência KL, Gini e ganho de informação nas árvores, e informação mútua |
| [16 · Inferência bayesiana](16_inferencia_bayesiana.ipynb) | Priori Beta e o modelo Beta-Binomial, encolhimento, intervalos de credibilidade, teste A/B bayesiano e o Ridge como uma priori normal |

**Extras:** depois de terminar a trilha principal, aprofunde com:

| Notebook | O que você aprende |
|---|---|
| [17 · Amostragem e viés](17_amostragem_e_vies.ipynb) | Amostragem estratificada e o `stratify=y`, viés de seleção (e por que mais dados não o corrigem), pesos IPW, pós-estratificação e viés de sobrevivência |
| [18 · Simulação de Monte Carlo](18_simulacao_de_monte_carlo.ipynb) | Estimar π e integrais, transformação inversa, simulação de risco com dados reais e valor esperado de uma decisão |

## 🛠️ Configurando o ambiente

### Pré-requisitos

- **Python 3.10 ou mais recente.** Para conferir sua versão:
  ```bash
  python3 --version
  ```
- **Git**, para baixar o repositório.

### 1. Baixe o repositório

```bash
git clone https://github.com/JoaoBLeite/ML-00-Fundamentos-estatistica-probabilidade.git
cd ML-00-Fundamentos-estatistica-probabilidade
```

### 2. Crie um ambiente virtual

Um **ambiente virtual** é uma pasta isolada com o Python e as bibliotecas **só deste projeto**. Assim, as versões instaladas aqui não interferem em outros projetos do seu computador, e vice-versa.

```bash
python3 -m venv .venv
```

Isso cria a pasta `.venv/` dentro do projeto. Ela não vai para o Git, porque já está no `.gitignore`.

> 💡 **No Ubuntu/Debian**, se aparecer um erro dizendo que o `venv` não está disponível, instale-o com:
> `sudo apt install python3-venv`

### 3. Ative o ambiente virtual

O ambiente precisa ser **ativado em cada novo terminal** que você abrir.

| Sistema | Comando |
|---|---|
| Linux / macOS | `source .venv/bin/activate` |
| Windows (PowerShell) | `.venv\Scripts\Activate.ps1` |
| Windows (Prompt de Comando) | `.venv\Scripts\activate.bat` |

Quando o ambiente está ativo, o nome `(.venv)` aparece no começo da linha do terminal. Para desativar, use `deactivate`.

### 4. Instale as bibliotecas

Com o ambiente **ativado**:

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

O arquivo `requirements.txt` lista as versões exatas usadas no projeto. As principais são:

| Biblioteca | Para quê |
|---|---|
| `numpy` | Cálculos numéricos e simulações |
| `pandas` | Manipular tabelas de dados |
| `scipy` | Distribuições de probabilidade, testes e otimização (`scipy.stats`, `scipy.optimize`) |
| `statsmodels` | Regressão com erros padrão, cálculo de poder, intervalos para proporções e testes múltiplos |
| `matplotlib` e `seaborn` | Gráficos (e os datasets tips e penguins) |
| `scikit-learn` | Comparações com os modelos de ML (logística, Ridge, PCA, árvores) |
| `jupyter` | Rodar os notebooks |

Para conferir se deu tudo certo:

```bash
python -c "import numpy, scipy, statsmodels, seaborn; print('Tudo instalado!')"
```

## ▶️ Como executar

### 1. Abra o Jupyter

Com o ambiente virtual **ativado**, na pasta do projeto:

```bash
jupyter notebook
```

O navegador vai abrir com a lista de arquivos do projeto. Se preferir uma interface mais completa, use `jupyter lab`.

> 💡 **Usa o VS Code?** Abra a pasta do projeto, abra um notebook e, no canto superior direito, escolha o *kernel* do Python que está em `.venv`.

### 2. Siga os notebooks em ordem

Comece pelo **01** e siga até o **16**. Cada notebook pressupõe os conceitos dos anteriores. O **17** e o **18** são extras, para depois da trilha principal.

Dentro de um notebook:
- **`Shift + Enter`** executa a célula atual e passa para a próxima.
- Execute as células **de cima para baixo**: uma célula pode depender de variáveis criadas nas anteriores.
- Para rodar tudo do zero: menu **Kernel → Restart Kernel and Run All Cells**.

### Observações

- **Na primeira execução**, os datasets tips e penguins são baixados da internet pelo seaborn e ficam salvos em `~/seaborn-data`. Nas próximas vezes, não é preciso conexão.
- **Todos os notebooks rodam em poucos segundos.** O mais demorado é o 17 (cerca de 20 segundos).
- As simulações usam **sementes fixas** (`np.random.default_rng(42)`), então os números das conclusões se repetem toda vez que você roda um notebook do começo ao fim.
- Os notebooks já estão salvos **com os resultados**, então dá para lê-los aqui no GitHub mesmo sem executá-los.

## 📁 Estrutura do projeto

```
ML-00-Fundamentos-estatistica-probabilidade/
├── 01_dados_e_tipos_de_variaveis.ipynb
├── 02_medidas_de_tendencia_e_dispersao.ipynb
├── 03_visualizando_distribuicoes.ipynb
├── 04_relacoes_entre_variaveis.ipynb
├── 05_fundamentos_de_probabilidade.ipynb
├── 06_probabilidade_condicional_e_bayes.ipynb
├── 07_variaveis_aleatorias_discretas.ipynb
├── 08_variaveis_aleatorias_continuas.ipynb
├── 09_distribuicoes_conjuntas.ipynb
├── 10_lei_dos_grandes_numeros_e_tcl.ipynb
├── 11_estimacao_e_intervalos_de_confianca.ipynb
├── 12_testes_de_hipotese.ipynb
├── 13_maxima_verossimilhanca.ipynb
├── 14_regressao_linear_estatistica.ipynb
├── 15_entropia_e_informacao.ipynb
├── 16_inferencia_bayesiana.ipynb
├── 17_amostragem_e_vies.ipynb            # extra
├── 18_simulacao_de_monte_carlo.ipynb     # extra
├── myst.yml              # configuração do livro (Jupyter Book)
└── requirements.txt      # bibliotecas e versões do projeto
```

## 📝 Como citar

Se usar este material, cite-o assim (ABNT):

> LEITE, João Pedro Barbosa. **Fundamentos de Estatística e Probabilidade para Machine Learning**. Zenodo, 2026. DOI: [10.5281/zenodo.23669967](https://doi.org/10.5281/zenodo.23669967).

Esse DOI sempre aponta para a versão mais recente. No GitHub, o botão **Cite this repository** gera a citação em outros formatos (APA, BibTeX).

## 📄 Licença

Este material está sob a licença [Creative Commons Atribuição-NãoComercial-CompartilhaIgual 4.0 Internacional (CC BY-NC-SA 4.0)](LICENSE): você pode copiar, adaptar e redistribuir, desde que cite a autoria, não use para fins comerciais e distribua as adaptações sob a mesma licença.
