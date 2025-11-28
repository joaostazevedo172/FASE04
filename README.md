# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="https://tse2.mm.bing.net/th/id/OIP.3xs_MSeNC0T1UOrJaCEqWAHaEK?cb=12&rs=1&pid=ImgDetMain&o=7&rm=3" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

## 👨‍🎓 Integrantes: 
- <a href="#">Maria Luiza Oliveira Carvalho</a> 
- <a href="#">Miriã Leal Mantovani</a>
- <a href="#">João Pedro Santos Azevedo</a> 
- <a href="#">Rodrigo de Souza Freitas</a>

## 👩‍🏫 Professores:
### Tutor(a) 
- <a href="https://github.com/SabrinaOtoni">Sabrina Otoni</a>

# 🌾 Classificação Automatizada de Grãos de Trigo

Projeto de Machine Learning aplicando a metodologia **CRISP-DM** para automatizar a classificação de variedades de trigo em cooperativas agrícolas.

---

## 📋 Sobre o Projeto

Em cooperativas agrícolas, a classificação de grãos é frequentemente manual, lenta e sujeita a erros. Este projeto busca resolver esse problema usando algoritmos de Aprendizado de Máquina para classificar **três variedades de trigo** com base em características físicas (geométricas).

**Objetivo:** Desenvolver um modelo preditivo capaz de distinguir entre as variedades **Kama**, **Rosa** e **Canadian** com alta precisão.

---

## 🗂️ O Conjunto de Dados (Dataset)

Dataset utilizado: **Seeds Dataset – UCI Machine Learning Repository**

- **Amostras:** 210 grãos (70 por variedade)  
- **Atributos (Features):**
  - Área  
  - Perímetro  
  - Compacidade `C = 4πA / P²`  
  - Comprimento do Núcleo  
  - Largura do Núcleo  
  - Coeficiente de Assimetria  
  - Comprimento do Sulco do Núcleo  

---

## ⚙️ Metodologia (CRISP-DM)

### **1. Entendimento e Preparação dos Dados**
- Análise Exploratória (Histogramas, Boxplots)
- Heatmap de correlação e Pairplot
- Padronização com **StandardScaler**

### **2. Modelagem**
- Divisão Treino/Teste: **70/30**
- Modelos treinados:
  - KNN  
  - SVM  
  - Random Forest  
  - Naive Bayes  
  - Regressão Logística

### **3. Otimização**
- Refinamento de hiperparâmetros via **Grid Search**  
  - Foco em **KNN** e **Random Forest**

### **4. Avaliação e Interpretação**
- Métricas analisadas: Acurácia, F1-Score, Matriz de Confusão  
- Estudo de Importância das Features

---

## 📊 Resultados Alcançados

### **Desempenho dos Modelos (Teste)**

| Rank | Modelo                     | Acurácia | F1-Score |
|------|-----------------------------|----------|----------|
| 🥇   | Random Forest (Otimizado)   | 92.06%   | 0.919    |
| 🥈   | K-Nearest Neighbors (KNN)   | 87.30%   | 0.871    |
| 🥉   | Support Vector Machine (SVM) | 87.30%   | 0.871    |

### **Principais Insights**
- O modelo **Random Forest** apresentou o melhor desempenho.  
- A feature **Compacidade** e as dimensões do núcleo foram essenciais para a classificação.  
- O sistema é viável para implantação e supera a consistência humana em tarefas repetitivas.

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3  
- **Ambiente:** Jupyter Notebook / VS Code  
- **Bibliotecas:**
  - `pandas` e `numpy` – Manipulação de dados  
  - `matplotlib` e `seaborn` – Visualização  
  - `scikit-learn` – Modelagem, pré-processamento, métricas  

---

## ▶️ Como Executar o Projeto

1. Clone o repositório ou baixe os arquivos  
2. Instale as dependências:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
