# 2022 Hacker Refactor Presentation

These are the materials for 2022 presentation I gave on R to OSU Cascade's
Hacker Refactor club.

You can run the notebook via jupyterlab in docker like so:

```
git clone https://github.com/joshkunz/2022-r-hacker-refactor-presentation presentation
cd presentation
docker run --rm -it -p 8888:8888 -v $PWD:/home/jovyan/work jupyter/datascience-notebook
```

The docker command will print a link to the jupyter lab instance to open
it in your browser.

## Run

## Converting to slides

```
docker run --rm -it -v $PWD:/home/jovyan jupyter/datascience-notebook jupyter nbconvert 2022-hacker-refactor.ipynb --to slides
```

## The "pokemon" dataset

This dataset can be obtained from [D0ltHub](https://www.dolthub.com/repositories/dolthub/pokemon)
as follows:

```
dolt clone dolthub/pokemon
cd pokemon
dolt table export pokemon pokemon.csv
```
