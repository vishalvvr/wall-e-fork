# Wall-E
Collector of absolute 3rd party packages from existing projects

![wall-e](https://www.looper.com/img/gallery/the-terrifying-detail-you-missed-in-wall-es-opening-scene/intro-1608234708.jpg)

## Background
This project aims to generate `requirements.txt` file for existing repositories where you have an old file which is filled with dependencies of dependencies. 

## Function
Wall-E uses `ast` module of python to parse nodes of any python script. Once the modules are retrieved, `pkg_resources` helps to find the right project name and version of the application installed. 

## Usage 
```python wall_e.py --project_folder /absolute/path/to/folder --exclude venv,__pycache__,__init__.py```

