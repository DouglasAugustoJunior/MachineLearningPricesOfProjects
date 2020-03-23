
# MachineLearningPricesOfProjects


![Project](https://img.shields.io/badge/MachineLearning-PricesOfProjects-blue)
![Version](https://img.shields.io/badge/Python-V1.0-blue)


Projeto utiliza a biblioteca **LinearSVC**, **SVC** e **StandardScaler** do **SKLEARN** para classificação e escala dos dados.
Também usa o **seaborn** e o **matplotlib.pyplot** para plotar os dados na tela.

O mesmo classifica os projetos finalizados e não finalizados com base no preço e horas esperadas.

Após fazer a leitura do arquivo CSV com os dados para classificação e fazer as alterações para melhor tratar os dados, assim como dividindo os mesmos para que seja possível treinar e testar, o projeto realiza o treinamento e verifica a acurácia obtida com o ***LinearSVC*** e com a ***baseLine*** (chute tudo 0 ou 1, para verificar o mínimo de acerto).
Após isso, ele plota os dados em um gráfico, onde *x = horas_esperadas* e *y= preco do projeto*.
Podemos verificar no console que a acurácia do algoritmo foi baixa, inferior a baseline.

![gráfico 1](https://github.com/DouglasAugustoJunior/MachineLearningPricesOfProjects/blob/master/Images/1.png?raw=true)

A segunda etapa exibe o segundo gráfico, além de exibir os dados também separa os mesmos por finalizado(laranja) ou não finalizado(azul).

![enter image description here](https://github.com/DouglasAugustoJunior/MachineLearningPricesOfProjects/blob/master/Images/2.png?raw=true)

A terceira etapa exibe 2 gráficos, onde separa os dados por finalizado e não finalizado.

![enter image description here](https://github.com/DouglasAugustoJunior/MachineLearningPricesOfProjects/blob/master/Images/3.png?raw=true)

Também é possível visualizar os dados em cores diferentes:

![enter image description here](https://github.com/DouglasAugustoJunior/MachineLearningPricesOfProjects/blob/master/Images/4.png?raw=true)

Ainda é exibido os dados somente do teste_x, para que seja comparado ao gráfico com todos os dados do CSV.

![enter image description here](https://github.com/DouglasAugustoJunior/MachineLearningPricesOfProjects/blob/master/Images/5.png?raw=true)

O próximo passo é exibir a curva de aprendizado do algoritmo, plotando os dados e a curva juntos no gráfico. Vemos que o *LinearSVC* não consegue atender a necessidade por se tratar de um algoritmo linear e nossa necessidade se tratar de uma curva,

![enter image description here](https://github.com/DouglasAugustoJunior/MachineLearningPricesOfProjects/blob/master/Images/6.png?raw=true)

Sendo assim, passamos a utilizar o SVC, para que seja possível corrigir a curva de aprendizado. Temos uma melhora na acurácia porém ao plotar o gráfico, ainda não temos uma curva de aprendizado satisfatória.

![enter image description here](https://github.com/DouglasAugustoJunior/MachineLearningPricesOfProjects/blob/master/Images/7.png?raw=true)

Isso ocorre porque, antes de treinar e verificar a acurácia do nosso algoritmo, precisamos corrigir a escala dos dados, o qual faremos utilizando o *StandardScaler*, dessa forma melhoramos nossa acurácia e também corrigimos nossa curva de aprendizado.

![enter image description here](https://github.com/DouglasAugustoJunior/MachineLearningPricesOfProjects/blob/master/Images/8.png?raw=true)
