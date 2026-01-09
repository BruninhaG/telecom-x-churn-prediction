# 📊 Análise e Previsão de Churn — Telecom X

## 📌 Objetivo do Projeto
Este projeto de **Machine Learning** tem como objetivo desenvolver um **modelo preditivo para identificar clientes com alto risco de evasão (churn)** na base de dados da empresa fictícia **Telecom X**.

O trabalho aplica conceitos fundamentais de **Ciência de Dados**, abrangendo desde o **pré-processamento dos dados** até a **avaliação e interpretação dos modelos**, com foco na geração de **insights acionáveis para o negócio**.

---

## 🏗️ Metodologia e Estrutura do Projeto
O projeto foi desenvolvido utilizando **Aprendizado Supervisionado**, seguindo as etapas abaixo:

### 🔧 1. Pré-processamento de Dados
- Carregamento e inspeção inicial do dataset  
- Remoção de colunas irrelevantes  
- Tratamento de valores ausentes  
- Codificação de variáveis categóricas  
- Normalização dos dados (quando aplicável)  

---

### 📊 2. Análise Exploratória de Dados (EDA)
- Investigação das principais características do conjunto de dados  
- Verificação do balanceamento das classes (churn vs. não churn)  
- Visualização de relações entre variáveis por meio de:
  - Boxplots  
  - Matriz de correlação  

---

### 🤖 3. Modelagem Preditiva
- Divisão dos dados em conjuntos de **treino** e **teste**
- Treinamento de dois modelos de classificação:
  - **Regressão Logística**  
    - Modelo simples e interpretável  
    - Sensível à escala (requer normalização)
  - **Random Forest**  
    - Modelo robusto  
    - Alto desempenho  
    - Não sensível à escala dos dados  

---

### 📈 4. Avaliação e Interpretação dos Modelos
Os modelos foram avaliados utilizando métricas padrão de classificação, com foco especial em **Recall** e **F1-Score**, por serem mais relevantes para o problema de churn.

#### 📊 Resultados no Conjunto de Teste

| Modelo              | Acurácia | Precisão | Recall | F1-Score |
|---------------------|:--------:|:--------:|:------:|:--------:|
| Regressão Logística | 0.8037   | 0.6558   | 0.5847 | 0.6183   |
| Random Forest       | 0.7963   | 0.6406   | 0.5977 | **0.6184** |

🔎 **Análise dos Resultados**

Embora a Regressão Logística tenha apresentado maior acurácia, o modelo **Random Forest** demonstrou desempenho ligeiramente superior nas métricas de **Recall** e **F1-Score**, que são especialmente relevantes para o problema de churn.

Esse resultado indica uma maior capacidade do modelo em identificar clientes que realmente cancelaram o serviço, reduzindo a ocorrência de **falsos negativos** e contribuindo para estratégias mais eficazes de retenção.

---

## 🔍 Principais Fatores Associados ao Churn
A análise de importância das variáveis revelou os seguintes fatores como os mais influentes na decisão de cancelamento:

1. **Tipo de Contrato**  
   Clientes com contratos **mensais** apresentam risco significativamente maior de evasão.

2. **Tempo de Contrato (Tenure)**  
   A probabilidade de churn é maior nos **primeiros meses de serviço**.

3. **Total Gasto**  
   Clientes com **menor valor gasto acumulado** tendem a cancelar com maior frequência.

---

## 💡 Recomendações Estratégicas
Com base nos resultados obtidos, recomenda-se como principal ação estratégica:

🎯 **Fidelizar clientes com contratos mensais e pouco tempo de permanência**, incentivando a migração para planos de maior duração por meio de:
- Ofertas exclusivas  
- Promoções direcionadas  
- Pacotes de benefícios personalizados  

Essa abordagem atua diretamente na **origem do churn**, contribuindo para o aumento da **retenção de clientes** e da **receita recorrente**.

---

## 🧠 Conclusão
O projeto demonstrou como técnicas de **Machine Learning** podem ser aplicadas para apoiar decisões estratégicas em empresas de telecomunicações.  
O modelo **Random Forest** se mostrou mais adequado ao contexto de churn, equilibrando desempenho técnico e impacto no negócio.

---

## 👩‍💻 Autora
Feito com 💛 por Bruna Guimarães

---

## 🌟 Apoie o projeto
Se você gostou, não esqueça de deixar um ⭐ no repositório! Isso ajuda muito o projeto a crescer e me incentiva a continuar criando. 🙌
