# smartsoccer
Project for predicting the outcome of soccer matches

# To use:
-Import the jupyter file(I recommend google colab)
-Use the datasets that are in the repository to train the algorithms


# Example of use:
model = modelGaussianNB

timeHome='Girona'
timeAway='Barcelona'

kicksAGolHome=5
kicksAGolAway=10

goalsHome=0
goalsAway=0

CurrentGame = [[golsHome,\
               goalsAway,\
               kicksAGolHome,\
               kicksAGolAway,\
               GetGrandezaCluster(timeHome),\
               GetGrandezaCluster(timeAway)]]
predictions = model.predict(currentgame)

Result = 'DRAW' 
