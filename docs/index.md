# 📚 Machine Learning 2025.2

<div align="center">

**Instrutor:** Humberto Sandmann  
**Última atualização:** 25 de Agosto de 2025  
**Repositório:** [GitHub](https://github.com)

</div>

---

## 📋 Índice

| Módulo | Tópico | Status |
|:-------|:-------|:-------|
| **1** | **Conceitos Fundamentais** | ✅ |
| 1.1 | [Machine Learning](#11-machine-learning) | ✅ |
| 1.2 | [KDD](#12-kdd) | ✅ |
| 1.3 | [Dados](#13-dados) | ✅ |
| 1.4 | [Exercícios](#14-exercícios) | ✅ |
| **2** | [Árvores de Decisão](#2-árvores-de-decisão) | 🔄 |
| **3** | [Pré-processamento](#3-pré-processamento) | ❌ |
| **4** | [KNN](#4-knn) | ❌ |
| **5** | [K-Means](#5-k-means) | ❌ |
| **6** | [Métricas de Avaliação](#6-métricas-de-avaliação) | ❌ |
| **7** | [Floresta Aleatória](#7-floresta-aleatória) | ❌ |
| **8** | [SVM](#8-svm) | ❌ |
| **9** | [PageRank](#9-pagerank) | ❌ |
| **10** | [PySpark](#10-pyspark) | ❌ |

---

## 1. Conceitos Fundamentais

### 1.1 Machine Learning

<div style="background: #f0f9ff; padding: 15px; border-radius: 8px; border-left: 4px solid #0369a1; margin: 15px 0;">

**Definição:** Machine Learning é um subcampo da inteligência artificial que se concentra no desenvolvimento de sistemas que podem aprender com dados.

</div>

**Tipos de Aprendizado:**
- ✅ **Aprendizado Supervisionado:** Modelos são treinados com dados rotulados
- 🔄 **Aprendizado Não Supervisionado:** Modelos identificam padrões em dados não rotulados
- ❌ **Aprendizado por Reforço:** Modelos aprendem através de tentativa e erro

### 1.2 KDD

<div style="background: #f0fdf4; padding: 15px; border-radius: 8px; border-left: 4px solid #15803d; margin: 15px 0;">

**KDD (Knowledge Discovery in Databases)** é o processo não trivial de identificar padrões válidos, novos, potencialmente úteis e compreensíveis nos dados.

</div>

**Etapas do KDD:**
1. Seleção de dados
2. Pré-processamento
3. Transformação
4. Mineração de dados
5. Interpretação/avaliação

### 1.3 Dados

<div style="background: #fffbeb; padding: 15px; border-radius: 8px; border-left: 4px solid #f59e0b; margin: 15px 0;">

Os dados são a matéria-prima fundamental para qualquer projeto de Machine Learning.

</div>

**Tipos de Dados:**
- **Estruturados:** Tabelas, bancos de dados relacionais
- **Não estruturados:** Texto, imagens, áudio
- **Semi-estruturados:** JSON, XML

### 1.4 Exercícios

<div style="background: #fdf2f8; padding: 15px; border-radius: 8px; border-left: 4px solid #ec4899; margin: 15px 0;">

**Exercício 1:** Explique a diferença entre aprendizado supervisionado e não supervisionado.

**Resposta:** 
O aprendizado supervisionado utiliza dados rotulados para treinar modelos, enquanto o não supervisionado busca padrões em dados não rotulados.

</div>

---

## 2. Árvores de Decisão

<div style="background: #faf5ff; padding: 15px; border-radius: 8px; border-left: 4px solid #8b5cf6; margin: 15px 0;">

**Status:** Em andamento 🔄  
**Data de estudo:** 25/08/2025

</div>

**Conceito:** Árvores de decisão são estruturas hierárquicas que representam regras de decisão.

**Vantagens:**
- Fáceis de interpretar
- Não requerem pré-processamento extensivo
- Lidam bem com dados numéricos e categóricos

**Algoritmos populares:**
- ID3
- C4.5
- CART

```python
# Exemplo de código para árvore de decisão
from sklearn.tree import DecisionTreeClassifier
from sklearn.datasets import load_iris

# Carregar dados
iris = load_iris()
X, y = iris.data, iris.target

# Criar e treinar modelo
clf = DecisionTreeClassifier()
clf.fit(X, y)