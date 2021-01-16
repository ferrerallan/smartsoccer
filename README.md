# smartsoccer
Projeto para predição de resultado de partidas de futebol

# Para utilizar:
-Importar o arquivo jupyter(recomendo google colab)
-Utilizar os datasets que estão no repositório para treinar os algoritmos


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
