
# Smart Soccer

## Description

Smart Soccer is a machine learning project designed to predict the outcomes of soccer matches. The project includes a dataset and a model, demonstrated with Jupyter notebooks, to help users understand and apply machine learning techniques in sports analytics.

## Requirements

- Python 3.7 or higher
- Jupyter Notebook
- Libraries: pandas, numpy, scikit-learn

## Mode of Use

1. Clone the repository:
   ```bash
   git clone https://github.com/ferrerallan/smartsoccer.git
   ```
2. Navigate to the project directory:
   ```bash
   cd smartsoccer
   ```
3. Open the Jupyter notebook:
   ```bash
   jupyter notebook
   ```
4. Load the provided datasets and execute the cells in the notebook to train and test the model.

## Example of Use

1. Define the model:
   ```python
   model = modelGaussianNB
   ```
2. Set up the match data:
   ```python
   timeHome = 'Girona'
   timeAway = 'Barcelona'
   kicksAGolHome = 5
   kicksAGolAway = 10
   goalsHome = 0
   goalsAway = 0
   ```
3. Prepare the input data:
   ```python
   CurrentGame = [[goalsHome, goalsAway, kicksAGolHome, kicksAGolAway, GetGrandezaCluster(timeHome), GetGrandezaCluster(timeAway)]]
   ```
4. Make predictions:
   ```python
   predictions = model.predict(CurrentGame)
   Result = 'DRAW' if predictions[0] == 0 else 'HOME WIN' if predictions[0] == 1 else 'AWAY WIN'
   ```

## License

This project is licensed under the MIT License.
