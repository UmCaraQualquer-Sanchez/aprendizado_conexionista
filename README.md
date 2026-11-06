FIA - Aprendizagem Conexionista

Aluno: Kauã de Souza Viana

05/11/2026

O código foi feito com base na página 30 do slide, onde temos um exemplo de treinamento de uma rede neural usando Python e a biblioteca NumPy.

A ideia do código é mostrar como uma rede neural consegue aprender ajustando seus pesos para diminuir o erro entre os valores que ela calcula e os valores esperados.

A rede possui uma camada de entrada com 1000 neurônios, uma camada oculta com 100 neurônios e uma camada de saída com 10 neurônios. Ela recebe 64 exemplos de treinamento, que são gerados aleatoriamente.

Durante o treinamento, o código faz os cálculos para obter uma saída e depois compara essa saída com o resultado esperado. Com isso, ele calcula o erro e utiliza os gradientes para ajustar os pesos da rede.

Esse processo se repete 2000 vezes, e a cada 100 repetições o código mostra o erro para acompanhar como a rede está aprendendo.

No teste realizado, o erro começou em aproximadamente 28257,81 e chegou a 4,96 na repetição 1900. Isso mostra que a rede conseguiu diminuir bastante o erro durante o treinamento.

O código não calcula diretamente a acurácia, pois não está trabalhando com uma classificação de dados. Nesse caso, o resultado é acompanhado pelo erro (loss), e quanto menor esse valor, mais próximas estão as saídas da rede dos valores esperados.

Com esse exemplo, conseguimos observar como funciona uma rede neural simples, como suas camadas são organizadas e como ela ajusta seus pesos durante o treinamento.
