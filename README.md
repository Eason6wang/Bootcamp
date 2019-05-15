# Bootcamp

The following instructions only apply to linux users

Some cheat sheets:

Conda: https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf

jupyter: https://www.cheatography.com/weidadeyue/cheat-sheets/jupyter-notebook/pdf_bw/

## Python
Open terminal, Type
```
python
```
You should get something like
```
Python 3.7.3 (default, Mar 27 2019, 16:54:48) 
[Clang 4.0.1 (tags/RELEASE_401/final)] :: Anaconda, Inc. on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```
Either python2 or python3 would be fine because anaconda will help manage versions

## Anaconda

WHY? It makes it easy to manage virtual environment, libraries and versions

Download Anaconda according to your python version from 
```
https://www.anaconda.com/distribution/
```
If you are using Mac, the export path would usually be added automatically. Check two shell scripts ~/.bashrc and ~/.bash_profile. As long as one of them contain something like
```
export PATH="...$PATH"
```
You are good to go!

### Virtual Environment
WHY? easy to perform version control
- Create environment
```
conda create --name YOUR_ENV_NAME INITIAL_LIB
```
YOUR_ENV_NAME: any name you like for your project

INITIAL_LIB: any library you want in your virtual environment

For example:
```
conda create --name OCR python=3.6 ipython jupyter
```
- Activate environment, so you can get in
```
conda activate YOUR_ENV_NAME
```
- Deactivate environment, so you can get out
```
conda deactivate
```

### Library
- Install libraries
```
conda install LIB=VERSION
```
if you want to install a specific branch of a github repo
```
pip install git+BRANCH_URL
```
- Test libraries
```
ipython
import LIB
# try some functions
```

### Jupyter
WHY? easy to share and interact with the code

Shortcuts:
- Shift-Enter -> run cell, select below
- Command-S -> save
Notes:

If your kenel is stuck in the middle of the process, make sure you "Save" first then click "close and halt" under "File" tab
