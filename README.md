# video-games-analysis

## Overview

This is your new Kedro project, which was generated using `Kedro 0.18.12`.

Take a look at the [Kedro documentation](https://kedro.readthedocs.io) to get started.

### Business problem

In 2017, the games industry made more money than the music industry and the movie industry combined! It's a fact that this entertainment niche is winning over more and more people every year. In Brazil, more than 66% said that they consume entertainment from the games niche.

The aim of the analysis is to create the following graphs and extract insights:

1. Histograms of the genres of the first 150 titles in the ranking.
2. Scatter plot between year of publication and Nintendo sales from 2010 onwards.
3. List of the top 5 publishers by sales in the United States.
4. Insight analysis.

Here is the [solution planning](docs/planning.md)

## Solution strategy
To solve the business problem I use the CRISP-DM methodology adapted for data science processes, the process steps for the solution will be as follows:

![crisp-method](/docs/crisp.png)

This process guarantees the construction of quick projects that allow potential problems to be visualized at every stage, as well as implementing continuous improvement with each new cycle.

## Notebook structure
The notebooks take advantage of Kedro's structure to be modular, allowing each stage of the solution to be a single notebook, the version in the notebook's name corresponds to the project cycle where each cycle represents a potential delivery for the interested party.
> Note: To ensure that the notebook runs, it is important to install the dependencies and run the notebooks sequentially.

## Rules and guidelines

In order to get the best out of the template:

* Don't remove any lines from the `.gitignore` file we provide
* Make sure your results can be reproduced by following a [data engineering convention](https://kedro.readthedocs.io/en/stable/faq/faq.html#what-is-data-engineering-convention)
* Don't commit data to your repository
* Don't commit any credentials or your local configuration to your repository. Keep all your credentials and local configuration in `conf/local/`

## How to install dependencies

Declare any dependencies in `src/requirements.txt` for `pip` installation and `src/environment.yml` for `conda` installation.

To install them, run:

```
pip install -r src/requirements.txt
```

## How to work with Kedro and notebooks

> Note: Using `kedro jupyter` or `kedro ipython` to run your notebook provides these variables in scope: `catalog`, `context`, `pipelines` and `session`.
>
> Jupyter, JupyterLab, and IPython are already included in the project requirements by default, so once you have run `pip install -r src/requirements.txt` you will not need to take any extra steps before you use them.

### Jupyter
To use Jupyter notebooks in your Kedro project, you need to install Jupyter:

```
pip install jupyter
```

After installing Jupyter, you can start a local notebook server:

```
kedro jupyter notebook
```

### JupyterLab
To use JupyterLab, you need to install it:

```
pip install jupyterlab
```

You can also start JupyterLab:

```
kedro jupyter lab
```

### IPython
And if you want to run an IPython session:

```
kedro ipython
```

## Conclusions
- We were able to extract information on market dominance in the PC market and Nintendo's share.
- We also found a strong market presence in titles for shooting and action games, which may indicate the type of behavior expected of the market, games that are frenetic.

## Next steps
- **Insight analysis**: We have a lot of hypotheses that could be analyzed by generos and markets.
- **Collecting data**: data from more platforms such as cell phones could provide a lot of insight and allow us to explore a new market.
- **Temporal analysis**: Using graphs and models to understand seasonal behavior, this would also require greater granularity of the time variable.
