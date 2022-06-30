# Natural-Language-Understanding-for-Multiple-Languages

Now you need to do the following steps, so you can use this rasa version 3.1 (I'm not ready testing 3.2, but it doesn't really matter) (with xlm):


Get poetry:
```bash
curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
```
make a conda enviroment and activate it (with pyhton 3.9 for example (works also with python 3.8)
```bash
make install
```

than you can (hopefully) run it :D

To run the config base on the german dataset, you can use this command:
```bash
rasa test nlu --nlu data_boris/data/annotatedGermanNLU.yml --config configs/config-base-german.yml --cross-validation --runs 1 --folds 5 --out gridresults/german/config-base
```
