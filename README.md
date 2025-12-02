# Residencia_IA_Detecao_Anomalias_SMAP
Trabalho Final da Residência em IA Aeroespacial - Classificação de Anomalias (NASA SMAP)
# 🛰️ Detecção de Anomalias em Telemetria Aeroespacial (NASA SMAP)

## 👤 Autor
Flávio José de Souza Bruno

## 🚀 Objetivo do Projeto
Este projeto implementa e compara modelos de Machine Learning Supervisionado (Random Forest e SVM) para a classificação em tempo real de anomalias em dados de telemetria do satélite NASA SMAP. O foco metodológico é a mitigação do risco operacional, priorizando a redução da taxa de Falsos Negativos (FN).

## 🛠️ Solução Técnica Utilizada
* **Modelo Vencedor:** Random Forest (Minimizou os Falsos Negativos: 56 FN).
* **Técnicas de Pré-Processamento:** RobustScaler (Normalização robusta) e SMOTE (Balanceamento de classes).
* **Ambiente de Execução:** Google Colaboratory (.ipynb).

---

## 💾 Instruções de Uso e Reprodução

1.  **Download do Código:** Clone este repositório ou baixe o arquivo `detecao_anomalias_nasa_smap.ipynb`.
2.  **Acesso ao Dataset:** O dataset utilizado é o **NASA Anomaly Detection Dataset SMAP & MSL** (Kaggle).
3.  https://www.kaggle.com/datasets/patrickfleith/nasa-anomaly-detection-dataset-smap-msl
4.  **Execução:** Abra o arquivo `.ipynb` no Google Colab e execute as células sequencialmente. O código trata automaticamente o acesso e a rotulagem dos dados.

## 📊 Resultados Chave (Análise de Risco)
A análise demonstrou que o Random Forest é o modelo mais seguro para a missão:

| Modelo | Falsos Negativos (FN) | Análise de Risco |
| :--- | :--- | :--- |
| **Random Forest** | 56 | **Recomendado:** Falhou menos vezes na detecção de anomalias reais. |
| **SVM** | 81 | **Risco Elevado:** Ignorou mais anomalias críticas. |

---
