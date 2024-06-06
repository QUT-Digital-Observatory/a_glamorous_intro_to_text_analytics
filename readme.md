# A Glamorous Introduction to Text Analytics

In this two-part workshop series, you will learn to collect posts from Reddit - using the very sparkly example of the Eurovision Song Contest - and apply a range of text analytic techniques to them. Some experience with R coding preferred, no experience with social media data collection or text analysis required.

## Running locally

Development and testing was done with Python version 3.12 and R version 4.4.

### Setup using Anaconda and RStudio

**TO WRITE**

### Setup using shell / command line interface

These instructions assume a little familiarity with installing and running Python packages from the command line, and that [Python](https://www.python.org/) and [R](https://www.r-project.org/) are already installed. All shell commands provided are run from this repository root directory.

We recommend creating and activating a new [Python virtual environment](https://docs.python.org/3/tutorial/venv.html).

Install Python requirements:

```shell
pip install -r python_requirements.txt
```

Open an R shell with:

```shell
R
```

Install [R notebook kernel](https://github.com/IRkernel/IRkernel):

```r
install.packages('IRkernel')
IRkernel::installspec()
```

To quit the R shell, use `q()` or the keyboard shortcut Ctrl+D (Cmd+D on Mac).

You may now as desired run individual notebooks with:

```shell
jupyter notebook 01_data_collection/explore.ipynb
```

Or you may as desired run a Jupyter Lab server for the whole project with:

```shell
jupyter lab
```

### Development

For additional setup steps for contributing code to this repository, see [CONTRIBUTING.md](CONTRIBUTING.md).


## Authors and license

Code and documentation by <span property="cc:attributionName">[QUT Digital Observatory](https://www.digitalobservatory.net.au/) and [the Language Technology and Data Analysis Laboratory (LADAL)](https://ladal.edu.au/)</span> and licensed under <a href="https://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY 4.0 <img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1" alt=""></a>

Support provided by [the Language Data Commons of Australia (LDACA)](https://www.ldaca.edu.au/) (and therefore [ARDC](https://ardc.edu.au/)) and the [QUT Library](https://www.library.qut.edu.au/).


