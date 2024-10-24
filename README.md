# 🏢 Projeto de Análise e Previsão de Turnover de Funcionários

Este é um projeto desenvolvido como parte do meu portfólio de ciência de dados, focando em análise de dados e machine learning para prever o turnover de funcionários em uma empresa. A análise foi realizada com base em um conjunto de dados hipotético, mas representa um problema real enfrentado por muitas organizações.

## 📋 Objetivo do Projeto

O objetivo principal é entender os fatores que influenciam os funcionários a deixarem a empresa e, com base nisso, criar um modelo preditivo que ajude o RH a identificar os funcionários com maior probabilidade de saída.

## 🚀 Tecnologias Utilizadas

- **Python** (principal linguagem)
- **Pandas** para manipulação de dados
- **Seaborn** e **Matplotlib** para visualização de dados
- **Scikit-learn** para implementação dos modelos de machine learning
- **BorutaPy** para seleção de variáveis importantes
- **SMOTE** para balanceamento de classes
- **Jupyter Notebook** para desenvolvimento interativo

## 📂 Estrutura do Projeto

O projeto foi dividido em várias etapas:

### 1. Descrição dos Dados

Começei com a análise inicial dos dados, onde foram descritas as colunas, dimensões, tipos de dados e valores ausentes. A base de dados inclui informações como idade, frequência de viagens, estado civil, salário e se o funcionário deixou a empresa ou não.

### 2. Criação de Hipóteses

Levantei 13 hipóteses sobre os fatores que poderiam influenciar a saída dos funcionários, como idade, satisfação no trabalho, formação, e equilíbrio de vida.

![Mapa de Hipóteses](https://iili.io/2FthJ0x.png)

Exemplo de hipótese: **Funcionários com salários mais baixos têm maior probabilidade de deixar a empresa.**

### 3. Análise Exploratória dos Dados

#### 3.1 Análise Univariada
Analisei as variáveis individuais, verificando a distribuição de categorias, valores nulos e outliers.

#### 3.2 Análise Bivariada
Testei as hipóteses levantadas e explorei a relação entre duas variáveis por vez. Por exemplo:

- **H1 (VERDADEIRA)**: Funcionários com menos de 30 anos têm maior probabilidade de sair da empresa.
- **H2 (FALSA)**: Funcionários com maior nível de formação têm menor probabilidade de sair.

![Análise Bivariada](link-para-imagem-analise.png)

#### 3.3 Análise Multivariada
Utilizei um heatmap de correlação para identificar as relações entre múltiplas variáveis, ajudando na escolha das variáveis mais relevantes para o modelo preditivo.

### 4. Pré-processamento dos Dados

- **Separação do conjunto de dados**: Dividi os dados em conjunto de treino e teste.
- **Balanceamento**: Usei a técnica de **SMOTE** para balancear as classes, já que havia mais funcionários que ficaram na empresa do que os que saíram.
- **Seleção de Variáveis**: Utilizei o **Boruta** para identificar as variáveis mais importantes para o modelo.

### 5. Modelagem

Implementei três modelos de machine learning para prever o turnover:

- **Regressão Logística**
- **Árvore de Decisão**
- **Random Forest**

A **Random Forest** e a **Regressão Logística** apresentaram a melhor performance em termos de Acurácia, ja a **Árvore de Decisão** teve melhor precisão em prever a saída dos funcionários (classe "Sim").

#### Resultados dos Modelos

| Modelo               | Acurácia | Recall Classe "Sim" |
|----------------------|----------|---------------------|
| Regressão Logística   | 84%      | 18%                 |
| Árvore de Decisão     | 73%      | 25%                 |
| Random Forest         | 84%      | 18%                 |

### 6. Conclusão

Através deste projeto, foi possível identificar os principais fatores que afetam a retenção dos funcionários. O equilíbrio de vida, o salário, e a satisfação no trabalho foram os maiores preditores de turnover. No entanto, ainda há desafios a serem resolvidos, como o desempenho em prever a saída da empresa, que pode ser melhorado com a otimização dos hiperparâmetros ou com a introdução de novos métodos de machine learning.

## 💡 O que aprendi

Este projeto me permitiu consolidar várias habilidades importantes, como:

- Manipulação e limpeza de dados com **Pandas**
- Visualização de dados com **Seaborn** e **Matplotlib**
- Criação e avaliação de modelos de machine learning com **Scikit-learn**
- Uso de técnicas como **SMOTE** para lidar com dados desbalanceados
- Seleção de variáveis importantes com o **BorutaPy**

## 📈 Próximos Passos

- Tentar novas técnicas de balanceamento de classes
- Explorar mais algoritmos de classificação
- Aplicar otimização de hiperparâmetros para melhorar o desempenho do modelo

## 📜 Licença

Este projeto está sob a licença MIT. Sinta-se à vontade para usá-lo como referência ou para aprender. 

## 🤝 Contribuições

Contribuições são sempre bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

## 📞 Contato

Se quiser discutir mais sobre o projeto ou tiver alguma sugestão, entre em contato comigo:

- Email: [alissonpereira.contato@gmail.com](mailto:alissonpereira.contato@gmail.com)
- LinkedIn: [linkedin.com/in/alisson-pereira-ds](https://www.linkedin.com/in/alisson-pereira-ds/)

---

Obrigado por conferir meu projeto! 😊
