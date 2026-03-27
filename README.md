# 🏦 Análise de Risco de Crédito com Dados Reais

## 📌 Visão Geral

Este projeto tem como objetivo analisar o risco de inadimplência utilizando um dataset real de crédito (German Credit Data), aplicando técnicas de **Análise Exploratória de Dados (EDA)**, **engenharia de features** e preparando a base para **modelagem preditiva de risco**.

A abordagem segue boas práticas utilizadas no setor financeiro, com foco em **interpretação de negócio e tomada de decisão**.

---

## 🎯 Objetivos

* Entender os principais fatores que influenciam a inadimplência
* Identificar padrões de comportamento entre bons e maus pagadores
* Criar variáveis relevantes para modelos de crédito
* Preparar a base para construção de score de crédito

---

## 📊 Dataset

* Fonte: German Credit Data (UCI / versão pública)
* Total de registros: 1.000 clientes
* Total de variáveis: 21
* Target: `Risk` (0 = bom pagador | 1 = inadimplente)

---

## 📂 Estrutura do Projeto

```
📁 projeto-risco-credito/
│
├── 01_EDA.ipynb                  # Análise exploratória completa
├── 02_Feature_Engineering.ipynb  # Criação de variáveis
├── 03_Modelagem.ipynb            # Modelo preditivo
│
└── README.md
```

---

## 🔍 Principais Análises Realizadas

### 📌 Análise Exploratória (EDA)

* Distribuição da variável target
* Análise de variáveis numéricas e categóricas
* Identificação de outliers
* Correlação entre variáveis
* Segmentação de clientes

### ⚙️ Feature Engineering

* Criação da variável `DebtRatio` (nível de endividamento)
* Padronização de dados
* Preparação para modelagem

### 🤖 Modelagem (base inicial)

* Random Forest Classifier
* Separação treino/teste
* Preparação para métricas de risco

---

## 🔎 Principais Insights

* ⚠ Base desbalanceada (70% bons vs 30% inadimplentes)
* ⏱ Maior duração de crédito → maior risco
* 💳 Endividamento (DebtRatio) é um dos principais drivers
* 📊 Variáveis categóricas possuem alto poder preditivo
* ↗ Créditos médios e altos apresentam maior inadimplência
* 🧠 Créditos muito altos possuem menor risco relativo (efeito de seleção)

---

## 🧠 Conclusão

A análise demonstra que o risco de crédito está diretamente ligado a:

* Comportamento financeiro do cliente
* Nível de exposição (valor e duração do crédito)
* Histórico de crédito

O projeto estabelece uma base sólida para evolução para:

* Modelos preditivos mais robustos
* Score de crédito
* Políticas de concessão

---

## 🚀 Próximos Passos

* Implementação de WOE (Weight of Evidence)
* Cálculo de IV (Information Value)
* Modelagem com Regressão Logística (padrão mercado financeiro)
* Avaliação com métricas como:

  * ROC / AUC
  * KS
  * Gini
* Construção de score de crédito

---

## 🛠 Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib / Seaborn
* Scikit-learn

---

## 💬 Sobre o Projeto

Este projeto foi desenvolvido com foco em demonstrar habilidades de um analista de dados atuando em contexto bancário, combinando:

* Análise técnica
* Interpretação de negócio
* Estruturação de pipeline analítico


---
