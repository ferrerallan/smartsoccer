# smartsoccer
Project for predicting the outcome of soccer matches 

# Para utilizar:
-Import the jupyter file(I recommend google colab)
-Use the datasets that are in the repository to train the algorithms 


# Exemplo de uso:
modelo = modeloGaussianNB

timeHome='Girona'
timeAway='Barcelona'

chutesAGolHome=5
chutesAGolAway=10

golsHome=0
golsAway=0

jogoAtual = [[golsHome,\
              golsAway,\
              chutesAGolHome,\
              chutesAGolAway,\
              GetGrandezaCluster(timeHome),\
              GetGrandezaCluster(timeAway)]]
previsoes = modelo.predict(jogoAtual)

Result = 'DRAW'
