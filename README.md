
# Transformer Translation Tutorial

Este repositório contém a implementação do tutorial do TensorFlow para tradução utilizando um modelo Transformer. O projeto demonstra a aplicação de técnicas de tradução automática, utilizando tokenização subword e um modelo Transformer treinado para traduzir do Português para o Inglês.


## Histórico de Commits

O versionamento deste projeto foi realizado através de pelo menos 3 commits significativos:

- **Commit 1 – Código Base Inicial:**  
  Adiciona o notebook com a implementação completa do tutorial, incluindo carregamento dos dados, criação dos tokenizers, preparação dos dados, definição do modelo Transformer, treinamento e avaliação.

- **Commit 2 – Ajustes no Treinamento e Inclusão de Métricas:**  
  Refatora o loop de treinamento com a criação da função `train_epoch`, que calcula a perda e a acurácia média por época, e implementa uma função simples de tradução para testes durante o treinamento.

- **Commit 3 – Adiciona gráficos de Loss e Acurácia:**  
  Registra o histórico de perda e acurácia para cada época e, ao final do treinamento, gera gráficos utilizando o matplotlib para visualizar a evolução dessas métricas.

## Pontos Positivos

- **Clareza e Modularidade:**  
  O código está organizado em células separadas, facilitando a leitura e a manutenção. Cada etapa (dados, treinamento, avaliação) está claramente definida.

- **Visualização das Métricas:**  
  A inclusão dos gráficos de Loss e Acurácia permite uma análise visual do desempenho do modelo ao longo do tempo.

- **Versionamento Significativo:**  
  O uso de commits com mensagens detalhadas possibilita o rastreamento das melhorias e alterações realizadas durante o desenvolvimento.

## Pontos Negativos

- **Desempenho em CPU:**  
  O treinamento utilizando CPU demonstrou ser muito mais lento, evidenciando que para tarefas com modelos complexos, o uso de GPU é praticamente indispensável para obter resultados em tempo razoável.

- **Complexidade do Modelo:**  
  O Transformer, embora poderoso, possui uma arquitetura complexa, o que pode dificultar a compreensão inicial para aqueles que estão começando a explorar redes neurais.

- **Dependência de Recursos Computacionais:**  
  A necessidade de um ambiente com GPU para treinamento eficiente pode limitar a experimentação em ambientes com hardware menos robusto.

## Avaliação de Desempenho (CPU vs GPU)

Durante o desenvolvimento, foi observado que o treinamento do modelo utilizando GPU apresenta uma performance muito superior em comparação com o treinamento em CPU. Embora não tenhamos registrado valores numéricos específicos, a diferença de tempo e eficiência foi evidente: o uso de CPU levou significativamente mais tempo e apresentou resultados piores em termos de iterações por segundo, confirmando a importância do hardware adequado para tarefas de deep learning.

---

