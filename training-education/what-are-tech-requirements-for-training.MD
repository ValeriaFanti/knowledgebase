# Copernicus Marine meets Jupyter for Training

![CopernicusMarine screenshot](https://github.com/copernicusmarine/copernicus-jupyter-notebook-gallery/blob/master/copernicus-marine-jupyter-overview.png "CopernicusMarine screenshot")

Copernicus Marine Trainings are "Users & Data Driven Discoveries", where we will use data as one driver (but not only) to discover new things. In order to do this discovery, we are going to need some tools to help us out. The most basic tool we will use is the Python programming language. At a later stage, we will use R programming language. We start with Python because it is a language that is particularly strong at processing data and has a massive number of libraries developed by its worldwide community that will help us achieving almost any needs.

There are least three ways to run Copernicus Marine Training contents:
1. On the cloud, [without installing anything](https://github.com/copernicusmarine/knowledgebase/new/master#no-installation), requiring only a web browser and internet connection
2. On your local machine, [installing only minimal requirements](https://github.com/copernicusmarine/knowledgebase/new/master#minimal-installation) for data science environment
3. On your local machine, [installing a complete powerful](https://github.com/copernicusmarine/knowledgebase/new/master#full-installation) data science environment

## No installation

Pass. _To be updated by June 2020 to display access to `Copernicus JupyterHub`._

## Minimal Installation

### Python - Miniconda3

Python itself is a programming language and you could install "just" Python. However, we want to use both Python and libraries that others have developed. For that, during Copernicus Marine Trainings, we will consume a Python distribution – a package that contains the Python programming language along side tools to make the process of getting libraries easier. Specifically, we will use the Miniconda distribution.

- Download: [Miniconda3 here](https://conda.io/miniconda.html)
- Need Help: 
  - [Right installer for your Operating System](https://conda.io/projects/conda/en/latest/user-guide/install/index.html)?
  - [Getting Started](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html)
  - [CheatSheet](https://conda.io/projects/conda/en/latest/_downloads/843d9e0198f2a193a3484886fa28163c/conda-cheatsheet.pdf)

### Copernicus Marine Environment

To create your Copernicus Marine Environment:
1. Open up the `Anaconda Prompt` command line interface and navigate to the directory of your choice._<br>**Note**: The default directory is ok, but it should be better to create a specific one, e.g. run:_<br>`python -c "import os; os.makedirs('copernicus')"; cd copernicus`<br>
2. To install the required modules, run this one line command:<br>
`conda create -n copernicus -c conda-forge python=3.7 jupyter xarray pathlib scipy matplotlib numpy pandas netcdf4 cartopy ftputil basemap openssl!=1.1.1e --yes`<br>
3. Once the `copernicus` environment is successfully installed, you should see something like:
```
[...]
cftime-1.1.1.1       | 225 KB    | ############################################################################ | 100%
[...]
#
# To deactivate an active environment, use
#
#     $ conda deactivate
```

4. Then activate the environment because we will need to issue one last command:

     `conda activate copernicus`

5. Finally, install the last required module by issuing:

     `pip install motuclient`

_<br>**Note**: Would you face any trouble in the process, please refer to [this article](http://marine.copernicus.eu/faq/what-are-the-motu-and-python-requirements/?idpage=169)_<br>


## Full Installation

### Python (and many more) - Anaconda Navigator
- Download: [Anaconda Navigator here](https://docs.anaconda.com/anaconda/install/)
- Need Help:
  - [User Guide](https://docs.anaconda.com/anaconda/user-guide/)
  - [CheatSheet](https://docs.anaconda.com/_downloads/9ee215ff15fde24bf01791d719084950/Anaconda-Starter-Guide.pdf)
  - [Frequently asked questions](https://docs.anaconda.com/anaconda/user-guide/faq/)

