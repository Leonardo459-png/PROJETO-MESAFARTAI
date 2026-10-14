1.	Informe quantos número de árvores foram utilizados no motor NLU. 
2.	Informa qual o valor de threshold foi utilizado no processo de limiar de confiança
3.	Coloque o resultado da primeira execução
4.	Descreva como você poderia fazer para os resultados de testes serem melhores, aumento o grau de confiança dos resultados
5.	Descreva por que o Random Forest foi o melhor método de Machine Learning para essa fase.

1. Foram utilizadas 80 árvores de decisão no algoritmo Random Forest, configuradas pelo parâmetro n_estimators=80.

2. O valor utilizado foi 0,60 (60%). Quando a confiança da previsão é inferior a esse limite, o sistema retorna uma resposta de fallback.

3. A primeira execução apresentou os seguintes resultados:
Frase de teste	Intenção retornada	Confiança
Tenho 30 kg de banana para doar	cadastrar_doacao	92,5%
Nossa instituição precisa de mantimentos	fallback	41%
Qual é a receita de bolo de cenoura?	fallback	49%
coisa comida doar la	fallback	42%
O modelo reconheceu corretamente a frase de doação com 92,5% de confiança. As outras três frases receberam fallback, pois apresentaram confiança inferior a 60% ou foram classificadas como fora do escopo.

4. Para melhorar os resultados, eu poderia aumentar a quantidade de frases utilizadas no treinamento, incluindo diferentes formas de pedir doações, solicitar alimentos e consultar o status dos pedidos.
5. O Random Forest foi escolhido porque utiliza várias árvores de decisão para realizar a classificação, combinando suas previsões. Isso ajuda a reconhecer padrões nas frases e pode reduzir o risco de depender de uma única árvore.

   
  
