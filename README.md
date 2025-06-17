# Comparação de Modelos Clássicos de Aprendizado Supervisionado na Classificação de Desempenho Escolar

## 1. Objetivo

Este projeto visa analisar, comparar e avaliar o desempenho de diferentes algoritmos de aprendizado supervisionado na tarefa de classificação binária do desempenho escolar, utilizando um conjunto de dados real extraído do [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Student+Performance). O pipeline foi desenvolvido para garantir reprodutibilidade, clareza e robustez, servindo como referência para projetos de análise preditiva em educação.

---

## 2. Conjunto de Dados

- **Fonte:** UCI Machine Learning Repository — Student Performance  
- **Arquivo:** `dataset/student-mat.csv`  
- **Instâncias:** 395  
- **Atributos:** 33 (demográficos, socioeconômicos, pessoais e de desempenho)  
- **Variável-Alvo:** `pass` (criada no pipeline)  
  - `1` para aprovado (nota final G3 ≥ 10)  
  - `0` para reprovado (nota final G3 < 10)  

---

## 3. Como Executar o Projeto

### 3.1 Pré-requisitos

- **Python 3.8+** instalado.
- Recomenda-se o uso de ambiente virtual (venv, conda, etc).

### 3.2 Instalação das Dependências

No terminal, navegue até a pasta do projeto e execute:

```bash
pip install matplotlib seaborn scikit-learn imbalanced-learn pandas numpy tensorflow
```

> **Observação:** O notebook já realiza a instalação automática das dependências na primeira célula, mas recomenda-se a instalação manual para evitar possíveis erros de ambiente.

### 3.3 Execução do Notebook

Você pode executar o notebook de duas formas:

#### Opção 1: Visual Studio Code

1. Abra o VS Code na pasta do projeto.
2. Abra o arquivo `main.ipynb`.
3. Execute as células sequencialmente clicando no botão de "play" ao lado de cada célula.

#### Opção 2: Jupyter Notebook

1. No terminal, execute:
    ```bash
    jupyter notebook
    ```
2. No navegador, abra o arquivo `main.ipynb` e execute as células na ordem apresentada.

### 3.4 Estrutura Recomendada de Pastas

```
neural-project/
│
├── main.ipynb
├── README.md
└── dataset/
    └── student-mat.csv
```

> **Importante:** Certifique-se de que o arquivo `student-mat.csv` está presente na pasta `dataset`.

---

## 4. Pipeline do Projeto

O pipeline contempla todas as etapas essenciais de um projeto de machine learning supervisionado:

1. **Coleta e tratamento de dados**
2. **Análise exploratória de dados (EDA)**
3. **Engenharia de atributos**
4. **Treinamento de múltiplos modelos**
5. **Avaliação comparativa**
6. **Análise de resultados e recomendações futuras**

---

## 5. Principais Etapas do Código

- Instalação e importação de bibliotecas
- Leitura e preparação do dataset
- Criação da variável-alvo (`pass`)
- Análise exploratória e visualização de dados
- Pré-processamento: codificação de variáveis categóricas (One-Hot), normalização (StandardScaler) e balanceamento (SMOTE)
- Divisão dos dados em treino e teste
- Treinamento dos modelos:
  - Árvore de Decisão
  - Random Forest
  - Rede Neural Artificial (Keras)
- Avaliação dos modelos: relatórios de classificação, matrizes de confusão, curvas ROC e métricas AUC

---

## 6. Boas Práticas e Diferenciais

- Pipeline modular, claro e facilmente reprodutível
- Sementes aleatórias fixadas para garantir reprodutibilidade dos resultados
- Pré-processamento padronizado para todos os modelos, assegurando comparabilidade
- Visualizações numéricas e gráficas para análise aprofundada
- Comparação direta e fundamentada entre diferentes algoritmos

---

## 7. Conclusão

Este pipeline oferece uma abordagem robusta, profissional e didática para análise de desempenho escolar utilizando aprendizado de máquina supervisionado. Permite:

- Tratamento de dados completo e confiável
- Aplicação e comparação de múltiplos algoritmos
- Avaliação justa e transparente de desempenho
- Apoio à compreensão dos fatores que influenciam o sucesso estudantil

---

## 8. Referências

- [UCI Machine Learning Repository — Student Performance](https://archive.ics.uci.edu/ml/datasets/Student+Performance)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)
- [TensorFlow/Keras Documentation](https://keras.io/)
- [Imbalanced-learn — SMOTE](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html)
