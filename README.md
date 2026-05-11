# 🩺 Diabetes Classifier (Machine Learning Model)

<img width="1536" height="1024" alt="Copilot_20260511_153059" src="https://github.com/user-attachments/assets/c32c395f-7738-49a2-8f6e-c352f2a9fba1" />


## 📘 Descrição
Este projeto aplica técnicas de **Machine Learning** para prever a probabilidade de um paciente desenvolver **diabetes tipo 2**, com base em variáveis clínicas e demográficas.  
O dataset utilizado é o clássico **Pima Indians Diabetes Dataset**, amplamente usado em estudos de classificação binária.

---

## 🎯 Objetivo
Construir um modelo capaz de **classificar pacientes** entre:

- **0 → Não diabético**
- **1 → Diabético**

Com base em atributos como:

- Número de gestações  
- Nível de glicose  
- Pressão arterial  
- Espessura da pele  
- Insulina  
- Índice de massa corporal (BMI)  
- Função de pedigree de diabetes  
- Idade  

---

## 📊 Dataset
- Fonte: [Pima Indians Diabetes Database - Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- Registros: 768
- Variáveis: 9 (8 preditoras + 1 alvo)
- Target: `Outcome` (0 ou 1)

---

## 🧪 Metodologia

### **1. Pré-processamento**
- Remoção de valores nulos  
- Padronização dos dados com `StandardScaler`  
- Separação entre features e target  

### **2. Divisão dos dados**
- 80% treino  
- 20% teste  
- `random_state=42` para reprodutibilidade  

### **3. Modelo**
O modelo utilizado foi o **Random Forest Classifier**, escolhido pela sua robustez e excelente desempenho em dados tabulares.

### **4. Avaliação**
- *Accuracy Score*  
- *Classification Report*  
- *Confusion Matrix*  
- Importância das features  

---

## 📈 Resultados

O modelo apresentou **alta acurácia** e boa capacidade de generalização.  
As variáveis mais relevantes foram:

1. **Glucose**  
2. **BMI**  
3. **Age**  
4. **Insulin**

A matriz de confusão mostrou bom equilíbrio entre classes, com leve tendência a falsos negativos — comum em problemas médicos onde a classe positiva é minoritária.

---

## 🛠 Tecnologias Utilizadas
- Python  
- Pandas  
- NumPy  
- Seaborn  
- Matplotlib  
- Scikit-Learn  

---

## ▶️ Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/alexpietz/diabetes-classifier.git
pip install -r requirements.txt
jupyter notebook diabetes.ipynb
