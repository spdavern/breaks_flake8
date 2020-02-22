# Summary

Installed jupyterlab-flake8:

```
$ conda install flake8
$ jupyter labextension install jupyterlab-flake8
$ jupyter labextension list
JupyterLab v1.2.6
Known labextensions:
   app dir: /usr/local/anaconda3/share/jupyter/lab
        @jupyterlab/git v0.9.0  enabled  OK
        @jupyterlab/github v1.0.1  enabled  OK
        @jupyterlab/toc v1.0.1  enabled  OK
        @lckr/jupyterlab_variableinspector v0.4.0  enabled  OK
        jupyterlab-drawio v0.6.0  enabled  OK
        nbdime-jupyterlab v1.0.0  enabled  OK
```

Reproduce Error:

1. Clone [this Github repo](https://github.com/spdavern/breaks_flake8) or [download this file](https://github.com/spdavern/breaks_flake8/blob/master/Hypothesis_test_review_and_power.ipynb)
2. Start jupyter lab (extension creates a terminal)
3. Create new notebook (linting works fine)
4. Open 'Hypothsis_test_review_and_power.ipynb' (error message appears - no kernel started for new notebook, jupyter lab unresponsive)