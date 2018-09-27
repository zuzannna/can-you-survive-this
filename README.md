# Can you survive this workshop? Brief introduction to survival analysis.
Co-authored by [Marianne Hoogeveen](https://github.com/marianneke) and [Zuzanna Klyszejko](https://github.com/zuzannna)

All you need to learn/teach basics of survival analysis. Deck & Python code with simulations, examples and more. Workshop originally delivered at Grace Hopper Celebration #GHC2018🌈👩🏾‍💻

## Handouts

There are 2 handouts that were given out during the workshop; they can be found in the `handouts` folder:
1. [`Breakout_Activity__Censoring.pdf`](handouts/Breakout_Activity__Censoring.pdf) asks the participants to classify several situations as either right censoring, left cenoring, or something else
1. [`Breakout_Activity__Blinking_Experiment.pdf`](handouts/Breakout_Activity__Blinking_Experiment.pdf) asks participants to perform an experiment in which one person tries go go as long as possible without blinking, and the experimenter notes their time in seconds, and whether they have any eyewear (contact lenses or glasses) or not.

## Example Notebooks 

There are 4 notebooks containing more details on concepts that were touched on during the workshop. You can view them in the browser but we encourage you to download them and play with numbers yourself. Here are some ideas you could start with: change distribution properties, add random (or not so random!) noise or use a completely different dataset. For example, there were [many datasets distributed with R package](http://vincentarelbundock.github.io/Rdatasets/) which you could use to play with Cox Proportional Hazards Model or to plot Kaplan-Meier curve. 

See `Dependencies and requirements` section at the end for installation tips.

### Survival Analysis Example

The notebook [`SurvivalAnalysisExample.ipynb`](example_notebooks/SurvivalAnalysisExample.ipynb) introduces several standard computational methods in survival analysis that are used to determine the effect of diverse factors on survival. For example, we used log rank test and Cox Proportional Hazards model on sample data set with the `lifelines` package in Python.

### Survival Function and Hazard Rate

The notebook [`SurvivalFunctionAndHazardRate.ipynb`](example_notebooks/SurvivalFunctionAndHazardRate.ipynb) shows the relationship between several important functions related to probability distributions one encounters for instance in survival analysis: the survival function, the hazard rate, the probability density function, and the cumulative density function.

### Censored survival data

The notebook [`CensoredSurvivalData.ipynb`](example_notebooks/CensoredSurvivalData.ipynb) illustrates the effect of having censored data, and why simply removing censored data is not the right thing to do.

### Survivorship Bias
The notebook [`SurvivorshipBias.ipynb`](example_notebooks/SurvivorshipBias.ipynb) illustrates the reverse problem with censored data: when _only_ censored observations are considered using an example of two gamblers with different strategies (high and low risk).

## Dependencies and requirements

If you have [Anaconda](https://docs.anaconda.com/anaconda/install/) (or [Miniconda](https://conda.io/docs/glossary.html#miniconda-glossary)) installed:

You'll need to install the `lifelines` package by typing the following comman in your command line (after cloning the repo and `cd` to the main repo directory):

```conda install -c conda-forge lifelines```

The notebooks also use software for making visualizations, such as `seaborn`:

```conda install seaborn```

Alternatively, you could use `pip install` to get all the packages once you clone the repo and type:

```pip install -r requirements.txt```

Finally, if you're new to Jupyter Notebooks, go [here](http://jupyter.org) to read the docs.
