# Wall-E
Collector of absolute 3rd party packages from existing projects

![wall-e](assets/img.jpg)

## Background
This project aims to generate `requirements.txt` file for existing repositories where you have an old file which is filled with dependencies of dependencies. 

## Function
Wall-E uses `ast` module of python to parse nodes of any python script. Once the modules are retrieved, `pkg_resources` helps to find the right project name and version of the application installed. 

## Install
```console
pip install 'git+https://github.com/FluffyDietEngine/wall-e'
```
or install from sources 
```
python3 setup.py install 
```

## Usage 
```console
wall-e --project_folder /absolute/path/to/folder --exclude venv,__pycache__,__init__.py
```