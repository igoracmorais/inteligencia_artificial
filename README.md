# Inteligencia Artificial

O uso de ferramentas de inteligência artificial não é recente, mas a verdade é que, com a maior acessibilidade a softwares e pacotes que permitem o uso de modelos mais elaborados na área, juntamente com a redução dos custos de processamento e armazenamento, criou-se o ambiente perfeito para impulsionar essa ciência. As aplicações são várias, indo desde modelos de previsão para o mercado financeiro até sistemas inteligentes que estão revolucionando o que entendemos como iteração com as máquinas.
Sem ter o intuito de esgotar o debate sobre o tema, esse projeto procura agrupar diversos notebooks do Python com exemplos de uso de ferramentas que envolvem duas importantes áreas da inteligência artificial, Machine Learning e Deep Learning.

## Classificação
Um problema de classificação envolve uma variável que contém classes (labels) e onde o modelo de previsão procura aproximar, a partir de uma função específica, as variáveis de input do conjunto de variáveis de output que são as classes. Os modelos de classificação, em inteligência artificial, são denominados de "aprendizado supervisionado" (supervised learning).

## Alguns algoritmos usados em classificação
Há diversos algoritmos em Machine Learning e Deep Learning que podem ser utilizados para problemas de classificação e fica difícil dizer qual deles performa melhor. Os resultados irão depender do tipo de problema que estamos avaliando e do comportamento dos dados. Abaixo discutimos rapidamente sobre alguns desses algoritmos.
### Árvore de decisão (Decision Tree - DT)
Nesse tipo de algoritmo, denominado de método de aprendizado supervisionado não paramétrico, temos que as decisões sobre o processo de classificação ocorrem no formato de árvore onde partimos de uma visão top-down. As decisões são feitas com base no if-then-else e é um algoritmo de fácil implementação e interpretação, mas é muito sensível a problemas de classificação do tipo imbalanced, onde uma classe tem mais dados que outra. Nesse caso, recomenda-se fazer um rebalanceamento das proporções dos dados antes de implementar o algoritmo. Outro problema com DT é quando temos muitas variáveis que representam as características (input) e que podem gerar um overfit dos dados.
### Support Vector Machine (SVM)
Esse método é muito eficiente em problemas de aprendizado supervisionado e pode ser aplicado tanto para regressão, classificação quanto para detecção de outliers. Uma das vantagens do uso do SVM é que temos diversos parâmetros que podem ser controlados, em especial a função kernel que irá produzir a divisão das classes.
### Naive Bayes (NB)
Esse algoritmo é baseado no teorema de Bayes e usado em problemas de aprendizado supervisionado assumindo que existe uma independência condicional entre os pares de valores das características e classes. Esse algoritmo pode ser usado com poucos dados de treino e para diversos problemas reais acaba produzindo resultados satisfatórios. Ele é muito utilizado para classificação de texto em análises do tipo NLP a partir da hipeotese de dados com distribuição multinomial.
### Ensemble
Esse é um método utilizado para otimizar o resultado da aplicação de diferentes algoritmos. A ideia é combinar diversos estimadores em apenas um. Isso pode ser feito de três formas. i) fazendo uma média de todos os estimadores usados, ou seja, selecionamos diferentes amostras. Podemos fazer isso a partir de dois modos, usando o Bagging (BaggingClassifier) ou o Forest of randomized trees, com RandomForestClassifier ou ExtraTreeClassifier; ii) Usa os estimadores de forma sequencial (boosting method) com o objetivo de reduzir o viés do estimador combinado. Podemos fazer isso a partir de dois modos. O primeiro usando o algoritmo AdaBoost ou então via Gradient Tree Boosting que possui a vantagem de ser um algoritmo robusto a presença de outilier e tem boa capacidade de previsão. E, por fim, podemos usar o iii) “voting classifier”. Aqui, aplicamos diferentes algoritmos de classificação e usamos um método de votação da maioria para escolher as classes que serão previstas. Recomenda-se o uso desse algoritmo para selecionar dentre diferentes modelos quando temos várias boas opções.

# Reinforcement Learning
Esse tema, também classificado na classe de modelos de Inteligência Artificial, explora uma forma diferente de aprendizado onde temos um agente que aprende com as mudanças que ocorrem no ambiente em que se encontra. Esse desenho acaba por gerar uma gama de aplicações interessantes como, carros autônomos, jogos, estratégias de marketing dentre outras. Veja que tanto os modelos de Machine Learning quanto os de Deep Learning são processos de aprendizado mas com foco em encontrar padrões nos dados. Por outro lado, os modelos de RL (Reinforcement Learning) atuam com tentativa e erro para aprender com os dados, e criamos uma recompensa pelo acerto que acaba criando como objetivo a maximização dessa receita. Isso posto, podemos definir quais são as peças que vão fazer parte da construção de um modelo de RL.
1. Estado: descreve a situaçao no qual o agente se encontra;
2. Açoes: esta relacionado ao conjunto de possibilidades de decisao que o agente pode fazer;
3. Ambiente: Descreve as caracteristicas do local onde o agente interage. Cada ambiente possui caracteristicas, recompensa e acoes diferentes;
4. Recompensa: nossa funçao objetivo que ira influenciar no algoritmo, dependendo do estado atual e futuro e da acao;
5. Politicas: conjunto de regras que define as escolhas do agente para suas acoes (agent brain).
Algumas referencias sobre RL
https://hub.packtpub.com/develop-stock-price-predictive-model-using-reinforcement-learning-tensorflow/
https://keon.io/deep-q-learning/
https://towardsdatascience.com/applications-of-reinforcement-learning-in-real-world-1a94955bcd12 
https://medium.freecodecamp.org/an-introduction-to-q-learning-reinforcement-learning-14ac0b4493cc
https://www.analyticsvidhya.com/blog/2017/01/introduction-to-reinforcement-learning-implementation/
https://medium.com/@gaurav1086/machine-learning-for-algorithmic-trading-f79201c8bac6
http://www.wildml.com/2018/02/introduction-to-learning-to-trade-with-reinforcement-learning/
https://github.com/kh-kim/stock_market_reinforcement_learning
https://quantdare.com/deep-reinforcement-trading/
https://github.com/edwardhdlu/q-trader
https://www.learndatasci.com/tutorials/reinforcement-q-learning-scratch-python-openai-gym/
