# Stock-Prices
Foram utilizados dois datasets nomeadamente: 
* historical_stock_prices
* historical_stocks

Obtidos em [Stock-Prices](https://www.kaggle.com/ehallmar/daily-historical-stock-prices-1970-2018?fbclid=IwAR0mkRuSU1u5GSJDSBPmKbAsJa1gnfJ7GSjYOxuSrqwMwFfNa0UgUzKfhUk)

## Objetivos
Com este estudo pretende-se realizar uma uma previsão do número stock prices e de quais os preços dos stocks tal como volumes de ações existem por empresas. Para além disso avaliar os setores das empresas predominantes no mercado como outros fatores.
Em primeiro lugar, tentar enriquecer o dataset com  todas as informações que conseguirmos encontrar que nos ajudem a melhorar a previsão dos stocks para determinadas empresas. 
Posteriormente utilizar vários modelos tradicionais de machine learning para prever estes stocks prices como modelos lineares, árvores de decisão e SVM.
Em segundo lugar, recorrer à utilização de DeepLearning, nomeadamente RNN para comparar resultados com o primeiro modelo e tirar conclusões.
Por último, proceder ao tunning dos nossos modelos e retirar conclusões pertinentes.

## historical_stocks


| 					  |  ticker  			|	exchange	|	name									|	sector	 		 |	industry				  |
| ------------------- | ------------------- | ------------- | ----------------------------------------- | -------------------| -------------------------- | 
|  0				  |  PIH				|	NASDAQ		|	1347 PROPERTY INSURANCE HOLDINGS, INC.	| FINANCE	 		 | PROPERTY-CASUALTY INSURERS |
|  1				  |  PIHPP				|	NASDAQ		|	1347 PROPERTY INSURANCE HOLDINGS, INC.	| FINANCE	 		 | PROPERTY-CASUALTY INSURERS |
|  2				  |  TURN				|	NASDAQ		|	180  DEGREE CAPITAL CORP.				| FINANCE	 		 | FINANCE/INVESTORS SERVICES |
|  3				  |  FLWS				|	NASDAQ		|	1-800 FLOWERS.COM, INC.		 			| CONSUMER SERVICES	 | OTHER SPECIALTY STORES 	  |
|  4				  |  FCCY				|	NASDAQ		|	1ST CONSTITUTION BANCORP (NJ)			| FINANCE	 		 | SAVINGS INSTITUTIONS 	  |

O dataset é constituido por 5 colunas:
* **ticker** corresponde ao nome das ações
* **exchange** corresponde ao tipo de troca efetuada
* **name** refere-se ao nome da empresa
* **sector** refere-se ao setor real em que a empresa em questão opera
* **industry** especifica o tipo de serviços que podem ser fornecidos pela empresa

## historical_stock_prices

| 					  |  ticker  			|	open	|	close	|	adj_close  |	low	 |  high  |  volume |    date      |
| ------------------- | ------------------- | --------- | --------- | ------------ | ------  | ------ | ------- | ------------ |
|  0				  |  AHH				|	11.50	|	11.58	| 	8.493155   |  11.25  | 11.68  |  4633900|  2013-05-08  |
|  1				  |  AHH				|	11.50	|	11.55	| 	8.471151   |  11.50  | 11.66  |  275800 |  2013-05-09  |
|  2				  |  AHH				|	11.50	|	11.60	| 	8.507822   |  11.50  | 11.65  |  277100 |  2013-05-10  |
|  3				  |  AHH				|	11.50	|	11.65	| 	8.544494   |  11.55  | 11.60  |  147400 |  2013-05-13  |
|  4				  |  AHH				|	11.50	|	11.53	|   8.456484   |  11.50  | 11.60  |  184100 |  2013-05-14  |
|  ...				  |  ...				|	...		|	...		| 	...		   |  ...    | ...	  |  ...	|   ...		   |
|  20973884			  |  NZF				|	14.60	|	14.59	| 	14.590000  |  14.58  | 14.62  |  137500 |  2018-08-20  |
|  20973885			  |  NZF				|	14.60	|	14.58	| 	14.580000  |  14.57  | 14.61  |  151200 |  2018-08-21  |
|  20973886			  |  NZF				|	14.58	|	14.59	| 	14.590000  |  14.57  | 14.63  |  185400 |  2018-08-22  |
|  20973887			  |  NZF				|	14.60	|	14.57	| 	14.570000  |  14.57  | 14.64  |  135600 |  2018-08-23  |
|  20973888			  |  NZF				|	14.60	|	14.69	| 	14.690000  |  14.59  | 14.69  |  180900 |  2018-08-24  |


O dataset é constituido por 8 colunas:
* **ticker** corresponde ao nome das ações
* **open** descreve o preço de abertura dessa ações num dia específico
* **close** descreve o preço final das ações no final de um dia
* **adj-close** descreve o preço ajustado de uma ações, que normalmente é diferente do preço de fecho da mesma
	- Um exemplo disto é quando ocorre uma divisão de stock. Um split de ações é a maneira utilizada pelas empresas para vender mais stocks, utilizando(x) como referência, se x = 2; se uma ação = 10 €, quando ocorrer o split, com um split = 2, a ação é igual a 5 €, mas no final essas 2 ações representam o mesmo que 1 ação, por exemplo, uma empresa tem 10 ações, se comprar 1 ação, terá 1% da empresa, num split de ações (split = 2), se comprar 2 ações, terá apenas 1% das duas empresas.
	- o preço das ações normalmente é afetado pela oferta e demanda dos participantes do mercado. No entanto, algumas ações corporativas, como split de ações, dividendos / distribuições e ofertas de direitos, podem afetar o preço de uma ação e são necessários ajustes para chegar a um valor tecnicamente preciso do verdadeiro valor dessa ação.
* **low** é o menor valor pago por essa ação
* **high** é o valor mais alto pago por essa ação
* **volume** representa o volume de ações compradas naquele dia
* **date** representa a data (ano-mês-dia)



# Algoritmos Machine Learning 

1. Linear Regression
2. Support Vectors Classifers for Regression SVR
3. Decisions Tree / Random Forest
4. Recurrent Neural Networks (RNN) / LSTM

# Grupo

* André Guilherme Nunes Viveiros - a81736
* Guilherme Marques Andrade – a80426
* Rodrigo Teixeira Pereira – pg38424


