# NLP - Análise de Sentimentos em Avaliações  

## Contexto  
Este projeto foi desenvolvido com fins **educacionais**, para praticar técnicas de **Processamento de Linguagem Natural (NLP)** aplicadas à análise de sentimentos em textos de avaliações.  

O objetivo é construir um pipeline que **classifique avaliações como positivas ou negativas**, aplicando desde o pré-processamento textual até a modelagem com **Regressão Logística**.  

---

## Tratamento e Preparação dos Dados  

### Pré-processamento de Texto  
- **Limpeza:** remoção de stopwords, pontuações e caracteres especiais.  
- **Tokenização:** divisão do texto em palavras.  
- **Normalização:** conversão para minúsculas, stemming ou lematização.  
- **Representação vetorial:**  
  - Bag of Words (BoW).  
  - TF-IDF para pesar termos mais relevantes.  

### Feature Engineering  
- Criação de matrizes esparsas com frequências de termos.  
- Testes com diferentes **n-grams** (bigramas, trigramas).  
- Comparação entre vocabulário reduzido e vocabulário completo.  

---

## Modelagem  

- **Algoritmo utilizado:** Logistic Regression  
- **Motivo da escolha:** modelo simples, interpretável e eficaz para problemas lineares de classificação de texto.  

### Avaliação  
- **Matriz de confusão** para análise de acertos/erros.  
- **Classification Report** com métricas de Precisão, Recall e F1-score.  
- **Curva ROC / AUC** para avaliar separação entre classes.  

---

## Resultados  

- O modelo apresentou **boa acurácia geral** e desempenho consistente.  
- **TF-IDF + Logistic Regression** foi a combinação com melhor equilíbrio entre performance e interpretabilidade.  
- **Principais erros:** frases irônicas ou avaliações ambíguas, difíceis de classificar apenas com tokens.   

---

## Tecnologias  

- **Python 3.11**  
- `pandas`, `numpy` – Manipulação de dados  
- `matplotlib`, `seaborn` – Visualização  
- `scikit-learn` – Vetorização (BoW, TF-IDF) e Regressão Logística  
- `nltk`, `spacy` – Processamento de texto  

---

Projeto desenvolvido como prática em **NLP aplicado à Análise de Sentimentos**, com o objetivo de exercitar:  
- **Pré-processamento textual**  
- **Feature Engineering em linguagem natural**  
- **Regressão Logística aplicada a texto**  
- **Avaliação de modelos com métricas de classificação**  
