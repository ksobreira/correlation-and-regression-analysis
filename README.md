# 📊 Análise de Correlação e Regressão Linear — DadosCorrel

Este projeto apresenta uma análise estatística completa utilizando o conjunto de dados **DadosCorrel**, desenvolvido no contexto da disciplina **Métodos Quantitativos para Ciências da Computação**.

O estudo investiga a relação entre duas variáveis quantitativas:

* **X (Velocidade)** → medida em rpm × 100
* **Y (Capacidade)** → medida em Horse Power (HP)

O objetivo é compreender o comportamento da capacidade da máquina em função da sua velocidade, utilizando técnicas estatísticas clássicas.

---

## 🎯 Objetivos do Projeto

* Visualizar a relação entre as variáveis através de gráfico de dispersão
* Calcular e interpretar o coeficiente de correlação de Pearson (Rxy)
* Estimar um modelo de regressão linear simples (MQO)
* Avaliar a qualidade do modelo com o coeficiente de determinação (R²)
* Verificar os pressupostos do modelo (normalidade dos resíduos)
* Validar o modelo por meio da ANOVA
* Realizar previsões com base no modelo ajustado

---

## 🧠 Fundamentação Teórica

A análise baseia-se em conceitos fundamentais de estatística:

* **Correlação de Pearson** → mede a força e direção da relação linear
* **Regressão Linear** → modela a relação entre X e Y
* **R² (Coeficiente de Determinação)** → indica o poder explicativo do modelo
* **ANOVA** → avalia a significância global do modelo
* **Testes de Normalidade** → verificam a adequação dos resíduos

---

## 🧪 Metodologia

O fluxo da análise segue as etapas abaixo:

1. Importação e tratamento dos dados
2. Análise exploratória (gráfico de dispersão)
3. Cálculo da correlação de Pearson
4. Ajuste do modelo de regressão linear (OLS)
5. Avaliação do modelo (R² e ANOVA)
6. Análise dos resíduos
7. Realização de previsões

---

## 📁 Estrutura do Projeto

```bash
project/
│
├── data/
│   └── raw/
│       └── DadosCorrel.xlsx        # Base de dados original
│
├── notebooks/
│   └── analysis.ipynb              # Notebook principal da análise
│
├── reports/
│   └── figures/                   # Gráficos gerados
│       ├── diagrama_dispersao.png
│       ├── regressao_linear.png
│       ├── histograma_residuos.png
│       └── qqplot_residuos.png
│
└── README.md
```

---

## 📊 Resultados Obtidos

### 🔗 Correlação

* **r ≈ 0,99**
* Indica uma **correlação linear positiva muito forte**

---

### 📈 Modelo de Regressão

Equação estimada:

```math
Y = 6{,}1203 + 2{,}6482X
```

**Interpretação:**

* A cada aumento de 1 unidade em X, Y aumenta em aproximadamente **2,65 HP**
* Relação direta e consistente entre as variáveis

---

### 📉 Coeficiente de Determinação

* **R² ≈ 0,968**
* O modelo explica aproximadamente **96,8% da variação de Y**

---

### 🧪 ANOVA

* **F = 662,1**
* **p-value ≈ 0,000**

✅ O modelo é estatisticamente significativo ao nível de 5%

---

### ⚠️ Normalidade dos Resíduos

* Teste indica **p < 0,05**
* Os resíduos **não seguem distribuição normal**

📌 Isso pode impactar inferências, mas não invalida o modelo para previsão

---

### 🔮 Previsão

Para:

```text
X = 25
```

Resultado:

```text
Y ≈ 72,33 HP
```

---

## 📈 Visualizações

O projeto gera:

* 📍 Diagrama de dispersão
* 📍 Reta de regressão
* 📍 Histograma dos resíduos
* 📍 QQ-Plot dos resíduos

---

## ⚙️ Tecnologias Utilizadas

* Python
* pandas
* numpy
* matplotlib
* seaborn
* scipy
* statsmodels
* openpyxl

---

## ▶️ Como Executar o Projeto

### 1. Clonar o repositório

```bash
git clone https://github.com/ksobreira/correlation-and-regression-analysis.git
```

---

### 2. Instalar dependências

```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels openpyxl
```

---

### 3. Executar o notebook

```bash
jupyter notebook
```

Abra o arquivo:

```bash
notebooks/correlacao_regressao.ipynb
```

---

## 📌 Contexto Acadêmico

Este projeto foi desenvolvido com base em uma atividade proposta na disciplina de **Métodos Quantitativos**, com o objetivo de aplicar técnicas estatísticas na análise de dados reais.


---

## 👨‍💻 Autor

Desenvolvido por **[Kauam Sobreira]**

---

## 📄 Licença

Este projeto é destinado exclusivamente para fins acadêmicos.
