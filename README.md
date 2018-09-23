# Can you survive this workshop? Brief introduction to survival analysis.
Marianne Hoogeveen, Zuzanna Klyszejko

All you need to learn/teach basics of survival analysis. Presentation &amp; sample analysis included. Originally delivered at Grace Hopper Celebration in Houston, 09/27/2018 #GHC2018👩🏾‍💻

```Recent years have seen a proliferation of algorithms to address tough data-related questions. However, in practice a model with clear interpretation is often preferable over a complex one. In this workshop we invite you to experiment with survival analysis to understand why is it used to predict phenomena such as lifetime of patients in healthcare, failure of computer chips and customer churn.```

## Example Notebooks 

There are 2 notebooks containing more details on concepts that were touched on during the workshop. In order to run them, you need to have [Anaconda](https://docs.anaconda.com/anaconda/install/) (or [Miniconda](https://conda.io/docs/glossary.html#miniconda-glossary)) installed.

After that is done, you'll need to install the `lifelines` package:
```conda install -c conda-forge lifelines```

The notebooks also use software for making visualizations, such as `seaborn`:
```conda install seaborn```

### Survival Analysis Example

The notebook [`SurvivalAnalysisExample.ipynb`](example_notebooks/SurvivalAnalysisExample.ipynb) introduces several standard computational methods in survival analysis that are used to determine the effect of diverse factors on survival. For example, the Cox Proportional Hazards model is used on sample data with the `lifelines` package in Python.

### Censored survival data

The notebook [`censored_survival_data.ipynb`](example_notebooks/censored_survival_data.ipynb) illustrates the effect of having censored data, and why simply removing censored data is not the right thing to do.
