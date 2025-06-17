# 💤 Quality of Sleep Prediction

Este projeto tem como objetivo prever a **qualidade do sono** de indivíduos com base em variáveis de estilo de vida e saúde, utilizando técnicas de **Machine Learning**.

## 📊 Dataset

- **Nome**: Sleep Health and Lifestyle Dataset  
- **Fonte**: [Kaggle - Sleep Health and Lifestyle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)  
- **Descrição**: Conjunto de dados com informações de 374 pessoas, incluindo idade, IMC, frequência cardíaca, nível de estresse, duração do sono, entre outros fatores.

---

## 🧪 Objetivo

Classificar a qualidade do sono em três categorias:
- `Ruim` (Quality ≤ 4)
- `Média` (entre 5 e 7)
- `Boa` (≥ 8)

---

## ⚙️ Etapas do projeto

1. **Análise exploratória de dados (EDA)**
   - Visualização da distribuição das variáveis.
   - Checagem e tratamento de valores nulos e duplicados.
   - Análise de outliers via boxplots.

2. **Pré-processamento**
   - Conversão de variáveis categóricas em numéricas.
   - Mapeamento manual da qualidade do sono para classes rotuladas.
   - Remoção de colunas irrelevantes.
   - Tratamento de outliers com base no IQR (para Heart Rate).

3. **Modelagem**
   - Separação dos dados em treino e teste com `train_test_split`.
   - Treinamento com `RandomForestClassifier` (modelo base).
   - Avaliação de performance usando:
     - Acurácia
     - Classification Report
     - Overfitting check (train vs test score)

4. **Visualizações**
   - Gráficos de barras para distribuição de distúrbios do sono.
   - Heatmap de correlação entre variáveis.
   - Boxplots individuais por coluna.

---

## 🧠 Modelo Utilizado

- **Algoritmo**: Random Forest Classifier
- **Métricas**:
  - Acurácia (test set)
  - Precision, Recall e F1-score (por classe)

---

## 📌 Principais variáveis usadas na predição

- Sleep Duration  
- Stress Level  
- Heart Rate  
- BMI Category  
- Physical Activity Level  
- Age  
- Gender  

---

## 📈 Resultados

- O modelo demonstrou **boas métricas de desempenho**, especialmente para classes bem representadas.
- A análise de correlação revelou que variáveis como **nível de estresse** e **frequência cardíaca** possuem relação significativa com a qualidade do sono.

