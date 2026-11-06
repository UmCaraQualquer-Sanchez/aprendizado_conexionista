# FIA - Aprendizagem Conexionista

Aluno: Kauã de Souza Viana

## Sobre o código

Nesse trabalho usei o código da página 30 do slide para testar o treinamento de uma rede neural em Python, usando NumPy. A rede recebe alguns valores, faz os cálculos e tenta chegar o mais perto possível do resultado esperado. A cada repetição, ela ajusta os pesos para diminuir o erro.

Os dados são criados de forma aleatória. Então o objetivo aqui é mais entender como a rede aprende do que resolver algum problema real.

## Camadas da rede

A rede é totalmente conectada e tem uma camada oculta. Ela é chamada de rede de 2 camadas no slide porque tem duas partes com pesos.

- Entrada: recebe 1000 valores.
- Camada oculta: tem 100 neurônios e usa a função sigmoide.
- Saída: produz 10 valores.

O código usa 64 exemplos. O `w1` liga a entrada à camada oculta, enquanto o `w2` liga a camada oculta à saída.

## Como funciona o treinamento

O treinamento acontece dentro do `for t in range(2000)`, ou seja, são 2000 repetições. Em cada uma delas, a rede calcula uma saída (`y_pred`) e compara com o valor esperado (`y`). Essa diferença é usada para calcular o erro (`loss`).

Depois, o código calcula os gradientes e atualiza os pesos. Assim, a rede vai tentando melhorar os resultados. Deixei o erro aparecendo a cada 100 repetições para não ficar mostrando tantos números.

## Resultados

No teste que ficou salvo no notebook, o erro começou em cerca de 28257,81 e chegou a 4,96 na repetição 1900. Dá pra perceber que ele foi diminuindo bastante durante o treinamento.

O código não mostra uma acurácia em porcentagem. Isso porque ele não está classificando imagens ou outras categorias, e sim tentando aproximar valores gerados aleatoriamente. Nesse caso, o que usamos para acompanhar o aprendizado é o erro (`loss`). Quanto menor ele fica, mais perto a saída da rede está dos valores esperados nesses exemplos.

## Como executar

É só abrir o arquivo `aprendizagem_conexionista.ipynb` no Google Colab ou no Jupyter e executar o código. Ele usa a biblioteca NumPy.
