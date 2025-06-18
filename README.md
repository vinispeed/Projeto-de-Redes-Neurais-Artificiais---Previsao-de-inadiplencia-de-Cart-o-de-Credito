# Projeto: Classificação de Inadimplência de Clientes

Este projeto tem como objetivo desenvolver, comparar e analisar modelos de machine learning para prever a inadimplência de clientes, utilizando redes neurais (Keras) e MLP do Scikit-learn.

## Objetivo

Prever se um cliente irá ou não entrar em inadimplência, auxiliando instituições financeiras na tomada de decisão de crédito e gestão de risco.

## Etapas do Projeto

1. **Análise Exploratória dos Dados**
   - Verificação de desbalanceamento das classes
   - Visualização e estatísticas descritivas

2. **Pré-processamento**
   - Limpeza dos dados
   - Normalização e transformação de variáveis

3. **Modelagem**
   - Treinamento de diferentes arquiteturas de redes neurais (Keras)
   - Treinamento de MLP com Scikit-learn
   - Teste de diferentes batch sizes, funções de ativação e learning rates
   - Avaliação do impacto de regularização (L2, Dropout)

4. **Avaliação**
   - Métricas: Acurácia, Precisão, Recall, F1-Score, AUC-ROC
   - Matrizes de confusão
   - Curvas ROC
   - Comparação direta entre os melhores modelos

5. **Análise dos Resultados**
   - Interpretação das métricas
   - Discussão sobre desbalanceamento e limitações
   - Recomendações para uso prático

## Principais Resultados

- O modelo Keras com arquitetura Large, função de ativação ReLU, batch size 64, learning rate 0.0001 e Dropout 0.5 apresentou o melhor desempenho geral.
- Ambos os modelos (Keras e Scikit-learn) são muito bons em identificar clientes adimplentes, mas têm dificuldade em identificar todos os inadimplentes (recall baixo para a classe minoritária).
- O modelo Keras apresentou leve vantagem em recall, F1-Score e AUC-ROC, sendo mais indicado para o objetivo de identificar inadimplentes.

## Como Reproduzir

1. Instale as dependências:
   ```
   pip install -r requirements.txt
   ```
2. Execute os notebooks ou scripts na ordem sugerida.
3. Analise os resultados gerados nas células de avaliação e gráficos.

## Limitações e Próximos Passos

- O desbalanceamento das classes impacta o recall para inadimplentes.
- Recomenda-se testar técnicas de balanceamento, ajuste de limiar e validação cruzada para maior robustez.
- Avaliar o impacto financeiro dos erros de classificação para melhor ajuste do modelo ao negócio.

## Contato

Para dúvidas ou sugestões, entre em contato pelo https://www.linkedin.com/in/marcos-vi-silva/.

---
Projeto desenvolvido para fins de estudo e demonstração de técnicas de classificação em problemas de risco de crédito.