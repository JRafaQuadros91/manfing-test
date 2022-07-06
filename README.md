Case Data Science Manfing - João Rafael Quadros

Preparação, Limpeza e Transformação dos dados.

Análise do Dataset, definição de objetivos e escolha/aplicação de modelo de Machine Learning.

Neste notebook estarei tratando a base de dados "DataSet_Test" que foram disponibilizados via e-mail.

Storytelling e anotações sobre o processo.

1 - Primeiramente foi realizada a Import das bibliotecas, configurado o ambiente e a importação do Dataset.

2 - Aqui realizamos uma análise descritiva desses dados, nesse ponto foi decidido por alterar o headers do Dataset para uma melhor visualização e entendimento durante o processo. Nessa etapa também foi verificado que existiam valores distoantes nas colunas Quantidade e Preço, será necessário resolver essa questão.

3 - Tratamento dos valores negativos para Quantidade e Preço e suposição do Dataset ser de um e-commerce bem variado em vários paises.

4 - Definido a estratégia de tratamento dos dados, dropar os dados nulos e negativos.

5 - Dados tratados e conferidos, passaremos a analisar os dados, suas variáveis , a dependência entre elas e definir planejamento, algumas métricas para visualização e modelos de Machine Learning aplicáveis.

6 - Após métricas e suas visualizações, será definido a abordagem e o/os algoritmos de machine learning aplicáveis para uma melhor análise e possível predição.

7 - Verificada a possibilidade de utilizar aprendizado supervisionado, escolhido os algoritmos de regressão linear e random forest, após comparações entre modelos e aplicação de machine learning, essa hipótese se tornou descartável, o modelo ficou underfiting, a correlação entre as variáveis do sub-dataset era irrelevante para que existisse uma correlação entre elas a ser utilizada para predições do algoritmo

8 - Seguiremos para a próxima ideia, Clustering, utilizaremos um modelo de associação.

9 - Dentre os metodos de k-means e apriori, o que chamou mais atenção foi o segundo , que teve uma boa confiança de associação de produtos em alguns deles (> 70%) o que poderia levar a estratégias da rede que vende os itens a elaborar promoções com esses itens, ou trabalhar com indicações de itens para associar com desconto.
Considerações.

Quanto ao tratamento dos dados, dataset não tinha muitos problemas, além de alguns produtos com descrição do tipo '???lost', mas eram pouquissimos casos, além de alguns dados duplicados, e com valores nulos, a opção foi dropar esses dados ao invez de substituir por alguma métrica como média, moda ou mediana
Seria possível metrificar e prever valores totais agrupando por clientes, seja criando grupos com intervalos classificando tipos de compradores, ou a relação dos clientes com o passar do tempo. Para isso seria necessário alterar os dados e agrupá-los e então tratar essas abordagens, assim , seria utilizado algum método de predição utilizando algoritmos de regressão.

Contudo , a abordagem foi utilizar o Dataset mais "naturalmente" com os dados da maneira que foram disponibilizados e trazer uma utilizade para eles, como se trata de alguma rede de supermercados ou coisa do tipo, acredito válida uma abordagem de associação, assim, poderiam se pensar várias estratégias para aumentar o lucro desde promoções envolvendo itens associados e indicações de itens que tem associação para adicionar ao carrinho de compras.
