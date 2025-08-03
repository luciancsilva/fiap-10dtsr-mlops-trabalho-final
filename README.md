## FIAP - MLOps - Trabalho Final

Este projeto foi desenvolvido como parte do trabalho final da disciplina de MLOps do MBA da FIAP. O objetivo é construir uma pipeline completa de Machine Learning que desenvolve um **score de crédito** a partir de dados históricos de clientes.

## 🎯 Objetivo

Desenvolver e publicar uma solução de score de crédito automatizada, com:

- Treinamento e comparação de múltiplos modelos de ML
- Registro e versionamento de experimentos com **MLflow** e **DAGsHub**
- Deploy da API via AWS
- Visualização da predição via aplicação em **Streamlit**

---

## 🧠 Modelos Treinados

Três algoritmos diferentes foram testados:

- `XGBClassifier`
- `LGBMClassifier`
- `DecisionTreeClassifier` ✅ **Melhor desempenho**

> O melhor modelo foi o **DecisionTreeClassifier**, escolhido com base em métricas como F1-score e acurácia ponderada.

---

## 🛠️ Ferramentas e Tecnologias

| Categoria           | Ferramentas                     |
|---------------------|----------------------------------|
| Gerenciamento de Experimentos | [MLflow](https://mlflow.org/), [DAGsHub](https://dagshub.com) |
| Frameworks de ML    | scikit-learn, xgboost, lightgbm |
| Visualização        | Streamlit                       |
| Armazenamento de Artefatos | DVC                        |
| Deploy da API       | AWS Lambda + Docker             |

---

## 📁 Estrutura do Projeto

Segue o padrão do [cookiecutter-data-science](https://drivendata.github.io/cookiecutter-data-science/):

```bash
├── data/               # Conjuntos de dados brutos e processados
├── models/             # Modelos treinados (.pkl)
├── notebooks/          # Notebooks de exploração e treino
├── src/                # Código da API
├── tests/              # Testes unitários
├── reports/            # Gráficos e relatórios
├── .dvc/               # Arquivos de versionamento DVC
├── requirements.txt    # Dependências do projeto
├── README.md           # Este documento

