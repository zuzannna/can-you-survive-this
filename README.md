# Can you survive this workshop? Brief introduction to survival analysis.
All you need to learn/teach basics of survival analysis. Presentation &amp; sample analysis included. Originally delivered at #GHC2018👩🏾‍💻


## Example Notebooks 

There are (?) notebooks containing more details on concepts that were touched on during the workshop. In order to run them, you need to have [Anaconda](https://docs.anaconda.com/anaconda/install/) (or [Miniconda](https://conda.io/docs/glossary.html#miniconda-glossary)) installed.

After that is done, you'll need to install the `lifelines` package:
```conda install -c conda-forge lifelines```

The notebooks also use software for making visualizations, such as `seaborn`:
```conda install seaborn```

### Censored survival data

The notebook [`censored_survival_data.ipynb`](example_notebooks/censored_survival_data.ipynb) illustrates the effect of having censored data, and why simply removing censored data is not the right thing to do.
