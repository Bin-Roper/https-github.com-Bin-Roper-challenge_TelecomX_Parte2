# 📊 Análise de Evasão 

Este projeto tem como propósito identificar os principais fatores que levam à evasão de clientes (churn) em uma empresa de telecomunicações, aplicando técnicas de aprendizado de máquina para desenvolver modelos preditivos robustos. Mais do que prever quem irá sair, a iniciativa busca compreender as causas por trás da decisão e sugerir estratégias eficazes de retenção.

---

## 💡 Objetivos

- Analisar o perfil dos clientes e identificar padrões de evasão.
- Aplicar técnicas de ML para prever o churn.
- Comparar o desempenho entre modelos Regressão Logística e Random Forest).
- Utilizar balanceamento de classes (SMOTE) para melhorar a equidade dos modelos.
- Gerar insights claros e aplicáveis para estratégias de retenção.

---

## 🧠 Modelos Utilizados

### 1. **Regressão Logística com SMOTE**
- Requer normalização dos dados.
- Bom para interpretar a influência de cada variável (coeficientes).
- Destaque para variáveis como `Encargos_Mensais`, `Encargos_Totais` e `Tempo_Servico`.

### 2. **Random Forest com SMOTE**
- Não exige normalização.
- Indicado para captar relações complexas entre variáveis.
- Destaque para `Tempo_Servico`, `Encargos_Totais`, e `Contrato_Conta`.

---

## 🔎 Principais Insights

### 🔥 Fatores que aumentam a evasão:
- Altos encargos mensais.
- Contrato mensal.
- Usuários de fibra óptica, mais veloz, porém com maiores custos e expectativas.
- Baixa fidelidade com a empresa.

### ❄️ Fatores que reduzem a evasão:
- Clientes antigos com maior tempo de vínculo.
- Usuários com contrato bienal.
- Clientes com dependentes e/ou parceiro no cadastro.

---

## 🛠️ Técnicas Aplicadas

- Pré-processamento: encoding, normalização.
- Balanceamento de classes com SMOTE.
- Ajuste de hiperparâmetros. (GridSearchCV)
- Métricas: Acurácia, Precisão, Recall, F1-score, e Matriz de Confusão.
- Análise interpretativa dos coeficientes e importâncias das variáveis.

---

## 📈 Métricas de Avaliação

| Modelo                       | Acurácia | Precisão | Recall | F1-score |
|-----------------------------|----------|----------|--------|----------|
| Regressão Logística (SMOTE) | 0.7611   | 0.5287   | 0.6578 | 0.5862   |
| Random Forest (SMOTE)       | 0.7652   | 0.5375   | 0.6257 | 0.5783   |

**Desempenho**: A regressão logística se destacou no recall, enquanto a random forest apresentou maior estabilidade geral.

---

## 🎯 Conclusão

A análise revelou que a evasão de clientes não é aleatória — ela segue padrões definidos de comportamento, relacionamento e percepção de valor. Quando corretamente interpretados, os modelos preditivos se transformam em ferramentas estratégicas para orientar ações mais personalizadas,  efetivas e mais condizentes às necessidades.

---

## 🧾 Requisitos

- Python 3.x
- pandas, numpy, matplotlib, seaborn
- scikit-learn, imblearn

---



