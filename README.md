# Challenge-Alura-TelecomX_BR-pt2
# 📊 TelecomX BR - Churn Prediction

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-green)
![Status](https://img.shields.io/badge/Status-Concluído-success)

Projeto de análise e modelagem preditiva para identificar **clientes com maior probabilidade de cancelamento (Churn)** em uma empresa de telecomunicações.

Este projeto foi desenvolvido durante a trilha de **Data Science do programa Oracle Next Education (ONE)** em parceria com a **Alura**.

---

# 🎯 Objetivo

O objetivo deste projeto é:

- Analisar os fatores que influenciam a evasão de clientes.
- Construir modelos de **Machine Learning** capazes de prever churn.
- Identificar **variáveis que impactam diretamente o cancelamento de serviços**.
- Propor **estratégias de retenção baseadas em dados**.

---

# 🗂 Estrutura do Projeto
```text
TelecomX_BR_pt2
├── dados_tratados.csv
├── TelecomX_BR_Parte2.ipynb
└── README.md
```


---

# 🛠 Tecnologias Utilizadas

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

# 📊 Análise Exploratória de Dados

Durante a análise exploratória foram investigados:

- distribuição de churn
- correlação entre variáveis
- relação entre **tempo de contrato e evasão**
- impacto dos **gastos totais e mensais**
- influência de **tipo de contrato e serviços contratados**

Também foi construída uma **matriz de correlação** para identificar os fatores mais relevantes.

---

# ⚙️ Modelagem Preditiva

Foram testados dois modelos principais:

- **Random Forest**
- **Regressão Logística**

E dois cenários de dados:

- Base original
- Base balanceada com **SMOTE**

A validação utilizou:

- Train/Test Split
- Cross Validation (K-Fold)

---

# 📈 Comparação de Modelos

| Modelo | SMOTE | Acurácia | Precisão | Recall | F1-score |
|------|------|------|------|------|------|
| Random Forest | Não | 0.78 | 0.62 | 0.46 | 0.53 |
| Regressão Logística | Não | **0.80** | 0.66 | 0.53 | 0.59 |
| Random Forest | Sim | 0.78 | 0.58 | 0.57 | 0.57 |
| **Regressão Logística** | **Sim** | 0.78 | 0.58 | **0.61** | **0.60** |

📌 **Melhor modelo:** Regressão Logística com SMOTE  
Ele apresentou o melhor equilíbrio entre **precisão e recall**, sendo mais eficiente para identificar clientes com risco de churn.

---

# 🔍 Principais Fatores de Churn

As variáveis mais associadas à evasão foram:

- Contratos **mensais**
- Uso de **fibra óptica**
- Método de pagamento **Electronic Check**
- **Paperless billing**
- Baixo **tempo de contrato (tenure)**

---

# 📉 Insights Obtidos

- Clientes com **contrato mensal** têm maior probabilidade de cancelar.
- Os **primeiros 12 meses** são o período mais crítico.
- Métodos de pagamento manuais estão associados a maior churn.
- Contratos de **1 ou 2 anos reduzem drasticamente a evasão**.

---

# 💡 Estratégias de Retenção Propostas

Com base na análise:

**1️⃣ Incentivar contratos de longo prazo**

Oferecer descontos ou upgrades para migrar clientes de planos mensais.

**2️⃣ Revisão do serviço de fibra óptica**

Investigar problemas de preço, qualidade ou suporte.

**3️⃣ Incentivo ao débito automático**

Reduzir churn associado ao pagamento manual.

**4️⃣ Programa de retenção para novos clientes**

Acompanhamento intensivo nos **primeiros 6 meses**.

---

# 🚀 Possível Aplicação

O modelo pode ser utilizado em um sistema de alerta para:

- identificar clientes com risco de churn
- priorizar ações de retenção
- reduzir custos de aquisição de novos clientes

---

# 📌 Conclusão

O modelo desenvolvido demonstrou capacidade de identificar padrões relevantes de evasão.

A aplicação de técnicas de **balanceamento de dados (SMOTE)** melhorou significativamente a capacidade do modelo de detectar clientes com risco de cancelamento.

A integração deste modelo em sistemas de CRM permitiria à empresa **agir preventivamente**, aumentando retenção e valor de vida do cliente.

---

# 👩‍💻 Autora

**Letícia Machado**

Projeto desenvolvido para fins educacionais no programa **Oracle Next Education (ONE)**.

