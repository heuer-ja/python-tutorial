


## Table of Contents
1. [About](#About)
1. [Interpreter](#Interpreter)
1. [Pip](#Pip)
	- [Commands](#Commands)
1.  [Anaconda](#Anaconda)
	- [Motivation](#Motivation)
	- [Miniconda vs. Conda](#Miniconda_vs._Conda)
	- [Commands](#Commands)
1. [Libraries](#Libraries)
1. [Packages](#Packages)
	- [MyPy](#MyPy)
1. [Editors & IDEs](#Editors_&_IDEs)
	- [PyCharm](#PyCharm)
	- [Spyder](#Spyder)
	- [Jupyter Notebook](#Jupyter_Notebook)
	- [Others](#Others)
  
  
## About Python  
Python is a general purpose programming language. 

### Usecases
- automation & scripting
- data science & machine learning
- backend (webdev.) 


## Interpreter
Interpreters for programming language *Python*.
Based on a interpreter some methods or versions of libraries may work or not.

-  **Python3.x** - state of the art
- Python2.x - deprecated

## Pip
Package-manager for installing python **libraries**.

### Commands
- install library *example* : `pip install example`

## Anaconda
- isolated *Python Enviroment* for programming.
- can use *pip*
 
### Motivation
-  **prevents crashing** system's python with programming installations
- installing/changing *python of OS* may lead to irreversible bugs
-  **switching** between different enviroments, each with custom settings
- python interpreter
- installed libraries
-  **no waiting** that a linux admin setups a enviroment on a server
- you can create an conda enviroment and export it

### Miniconda vs. Conda
| Miniconda | Conda |
|--|--|
| light weight | heavy weight (3GB) |
| install libs on demand| 1500 pre-installed libs|
| libs are up to date due to self-management| libs are outdated quickly|

### Commands
-  **version**: `conda -V`
-  **list** all conda enviroments: `conda env list`
-  **create** env.: `conda create -n NAME python=3.8 numpy`
-  **create** env. from .yaml: `conda env create --file NAME_OF_FILE.yml`
-  **delete** env. *example* : `conda remove -n exmaple --all`
-  **activate** env. *example*: `conda activate example`
-  **deactivate** an env.: `conda deactivate`
-  **install** package *example* in env: `conda install example` or `pip install example`
-  **export** current env.: `conda env export --name NAME_OF_ENV > NAME_OF_ENV.yml`

### Windows 11: Connect VS Code to Anaconda Jupyter Kernels
2022 Nov 29
Problem: It may happen that VS Code connects **only** to Jupyter Kernel installed on your real machine. Accordingly, it is not possible to choose any other Anaconda Kernels even though they are shown under Command Palette (CTRL + SHIFT + P) "Select: Python Interpreter".
Solution: Open Command Palette (CTRL + SHIFT + P) and type 'Jupyter: Filter Kernels'. Now, two things are possible to do: (A) uncheck the check box for the native Interpreter (that worked for me), or (B) insert following code

<code>
"jupyter.kernels.filter": [
      {
        "path": "/bin/python3"
      }
    ]
<\code>

### Sources
- https://www.youtube.com/watch?v=1VVCd0eSkYc&t=2s
  
## Libraries
- **numpy** - efficient arrays + operations
- **matplotlib** - vizualisations, customizable graphs, exports
- **scipy** - scienctific functions for maths. divided into subpages, each dealing with another topic (stats, lina, io)
- **pandas** - effiecent datastructures for .csv-files and multidimensional data
- **tensorflow** - machine learning
- **huggingface** - nlp 

## Packages
### MyPy
Works like a compiler and checks code for correct typing.

**Commands**
- normal: `mypy NAME_SCRIPT.py`
- ignoring imports: `ypy NAME_SCRIPT.py --ignore-missing-imports --follow-imports=skip`

**Flags**
 - ignoring missing imports: `--ignore-missing-imports`
 - follow imports: `--follow-imports=skip` 
 
 **Limits**
 - no multi assignment supported

## Editors & IDEs

### PyCharm
- most desired IDE in python community
- VS Code for Python
	---> complicated
- many plugins
- autocompletion

  

### Spyder
light-weight editor for data science, but no scalable extensions
  
 
### Jupyter Notebook
- interactive python text editor with *major vizualisation characteristic*.
- presenting data science scripts.
- run independent python cells
- vizualisation for graphs, datastructures, prints, ..

  

**Start Jupyter Notebook**

- from terminal: `jupyter notebook`

  

**Shortcuts**

- tab completion: `Tab`

- run cell: `CTRL` + `ENTER`

- new cell: `ESC` + `ENTER`

  
  
### Others
not appropriate but still o.k. alternatives are better
- VS Code
- Sublime
- ... 
