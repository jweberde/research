# My Notes on Python Setup

```bash
brew install pyenv
brew install pyenv-virtualenv
```

```bash
pyenv init
# make necessary changes to .zprofile
```

```
pyenv install 3.10.7
```

```bash
pyenv shell 3.10.7
pip install --upgrade pip
```

## Install jupyter

```bash
# Create virtual env for jupyter
pyenv virtualenv 3.10.7 jupyter
pyenv activate jupyter
pip install jupyterlab
```

### Setup Project

```bash
pyenv virtualenv 3.10.7 project_name_env
mkdir project_dir_source
cd project_dir_source
pyenv activate project_name_env
pyenv local project_name_env
````

Install some basics

Pandas — so we can manipulate data
Jupyter, Notebook and Ipykernel — so that we can use Jupyter Notebooks to write, execute and annotate code
Matplotlib and Seaborn for data visualizations.
Inside of your project directory, you can start the installation with Pip:

```bash
pip install pandas jupyterlab jupyter notebook ipykernel matplotlib seaborn voila
```

Create a kernelspec to start using virtual environments with Jupyter notebooks

To create a kernelspec for your virtual environment, enter the following in your project folder and make sure the environment is activated when you do it:

```bash
python -m ipykernel install --user --name taie --display-name "Python (taie)"
```

Start Notebook (classic) or Lab (newr)

```bash
jupyter lab
```

## Requirements

There is no such thing as package.json or build.gradle

```
pip freeze > requirements.txt 
```

```
pip install -r requirements.txt 
```
