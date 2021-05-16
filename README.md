# Beer Analysis
Analysis of the beer dataset by Oleg Żero [zerwithdot.com](https://zerowithdot.com).

## Project setup
The project uses python 3.9. You need to have it installed on your machine.
In order to run you need for fetch the dataset (requires setting up an account at Data World)
and creating a virtual environment.

### Fetching the dataset
Go over to [Data World](https://data.world/socialmediadata/beeradvocate), download the dataset and place
it under `data/beer.csv` directory or use the script.
```
cd scripts
./get_data.sh
cd ..
```
Make sure it has the right link.

### Run the notebooks
```
python3.9 -m venv env
source env/bin/activate
pip install -r requirements.txt

jupyter notebook
```

## Content
There are two notebooks there.
The `initial-exploration.ipynb` explores and cleans the dataset.
It also creates a new, processed dataset under `data/beer-processed.pkl`.
Then, the `questions-andwering.ipynb` is the actual answers to the questions.
It requries the previously generated file.

