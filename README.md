# Simulações de Monte Carlo Usando Python 
Repositório com notas de aula do curso realizado na plataforma DataCamp sobre implementar Simulações de Monte Carlo usando Python
# Bibliotecas Utilizadas 
  <img src="https://img.shields.io/badge/Numpy-4F0599?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/SciPy-654FF0?style=for-the-badge&logo=SciPy&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" /> 
  <img src="https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252"/>

# O que é a Simulação de Monte Carlo 

Dentro do trabalho de (PAULA,R.R,2014), encontramos a seguinte definição para o Método de Monte Carlo: "Uma definição formal de Método de Monte Carlo foi dada por Halton (1970). Ele definiu o método como uma técnica para representar a solução de um problema como um parâmetro de uma população hipotética e, que usa uma sequência aleatória de números
para construir uma amostra da população da qual estimativas estatísticas desse parâmetro possam ser obtidas". 

Tal método foi elaborado por John von Neumann e Stanislaw Ulam  no Projeto Manhattan, durante a construção da Bomba Atômica, Ulam e von Neumann consideraram a possibilidade de usar o método, que envolvia a simulação direta de problemas de natureza probabilística relacionados com o coeficiente de difusão do nêutron em certos materiais. 

O método recebe seu nome devido à prática comum de utilizar aleatoriedade e repetição, características das atividades de jogo em cassinos de Monte Carlo, Mônaco. Utilizado há bastante tempo, o método, ou processo, de Monte Carlo é empregado para obter aproximações numéricas de funções complexas. Geralmente, esses métodos envolvem a geração de observações de uma distribuição de probabilidades e o uso dessas amostras para aproximar a função de interesse. Além disso, o método é conhecido como simulação estocástica, sendo uma abordagem relativamente simples e de implementação fácil.

Em princípio, métodos de Monte Carlo podem ser usados para resolver quaisquer problemas com um interpretação probabilística. Pela Lei dos Grandes Números, integrais descritas pelo valor esperado de alguma variável aleatória podem ser aproximadas obtendo a média empírica de amostras independentes de variáveis. Quando a distribuição de probabilidade da variável é parametrizada, normalmente é utilizada o gerador de amostras Markov chain Monte Carlo (MCMC), tendo assim, que no limite, as amostras geradas serão amostras da distribuição desejada.

O Método de Monte Carlo é frequentemente usado nas seguintes áreas de conhecimento: 
* Finanças: Preço de Ações, Gestão de Risco.
* Física: Identificação da ligação em Proteínas
* Engenharia: Modelagem Mecânica de Sistemas físicos, simula probabilidades de falha e definir domínios de segurança

Támbem pode ser usado para estimar constantes, com base em parâmetros geométricos, como por exemplo o valor de $\pi$:
![Estimando o valor de $\pi$ usando Monte Carlo](https://github.com/luizmarioags/Python-Monte-Carlo/blob/main/Imagens/pi.png)


Tal método possui muitos benefícios em ser utilizado, como podemos citar: 
* Leva em consideração uma faixa de valores para várias entradas
* Não mostram somente o que poderia acontecer, mas a probabilidade de cada resultado
* Facilitam a criação de gráficos com a gama de resultados possíveis em um cenário
* Permitem examinar o que teria acontecido em diferentes circunstâncias

O Processo ou método de Monte Carlo pode ser resumido nos seguintes aspectos: 
* Definimos as variáveis de entrada e escolhemos as distribuições de probabilidade corretas para essas variáveis
* Geramos entradas por amostragem dessas distribuições
* Realizamos um cálculo determinístico das entradas simuladas
* Resumimos os resultados

Neste repositório você vai poder encontrar vários tipos de exemplos de como implementar esse método, além de construir pair plots que nos ajudam a verificar as relações de correlação entre as mais diversas variáveis dos nossos conjuntos de dados de interesse, como por exemplo, a relação entre as variáveis de Preço e Tamanho de uma casa. Além de gerar Mapas de Calor para compreender essas relações também:

![Pairplot para as variáveis de Preço e Tamnho de uma Casa](https://github.com/luizmarioags/Python-Monte-Carlo/blob/main/Imagens/normal_multivariada_pairplot.png)

![Cluster Map](https://github.com/luizmarioags/Python-Monte-Carlo/blob/main/Imagens/cluster_correlacao.png)

Além de gerar: 
* Distribuições de probabilidade discretas como a Geométrica:

![Distribuição Geométrica Simulada](https://github.com/luizmarioags/Python-Monte-Carlo/blob/main/Imagens/dist_geometrica.png)

* Distribuições Contínuas, como a Normal:

![Distribuição Normal Simulada](https://github.com/luizmarioags/Python-Monte-Carlo/blob/main/Imagens/dist_normal.png)

![Distribuição Normal Simulada](https://github.com/luizmarioags/Python-Monte-Carlo/blob/main/Imagens/sim_alturas.png)

# Dados Utilizados
O conjunto de dados utilizado neste repositório é o conjunto clássico sobre Diabetes, elaborado por Efron, Bradley & Hastie, Trevor & Johnstone, Iain & Tibshirani, Rob. (2004) em seus estudos sobre Diabetes, analisando  a progressão da doença em relação às mais diversas variáveis.

# **Referências Bibliográficas**

Efron, B.; Hastie, T.; Johnstone, I.; Tibshirani, R. Least angle regression (with discussions). *The Annals of Statistics*, v. 32, 2004.

PAULA, Renato Ricardo de et al. Método de Monte Carlo e aplicações. 2014

Ross, S. Probabilidade: Um Curso Moderno com Aplicações. Bookman, 2009. Disponível em: [https://books.google.com.br/books?id=ZKXtwsmyPFcC](https://books.google.com.br/books?id=ZKXtwsmyPFcC). Acesso em: 14 de abril de 2024.

Weber, I. Monte Carlo Simulations in Python. DataCamp, [Online Course](https://www.datacamp.com/courses/monte-carlo-simulations-in-python), acessado em: 14 de abril de 2024.
