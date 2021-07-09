# Contributing to [project name]

## Overview
Please note our general guidelines for contributing to NDCLab projects [here](https://ndclab.github.io/wiki/docs/contributing.html).

* [Roadmap](#Roadmap)  
* [Directory-Structure](#Directory-Structure)  
* [Scripts](#Scripts)
* [Containers](#Containers)  
* [Workflow](#Workflow)  

## Roadmap
Please see the roadmap available on the [README.md](https://github.com/NDCLab/template-tool/blob/main/container/README.md) file of this repository.

## Directory Structure
```yml
project-name
├── run.py
├── scripts
|    ├──__init__.py
├── container
|    ├──Dockerfile.template 
|    ├──environment.yml
|    ├──README.md 
├── .github 
```

### Scripts
The `scripts` directory is the local [package](https://docs.python.org/3/tutorial/modules.html#packages) where Python modules will be written in. This ensures that modules are neatly divided according to responsibility, which helps with parallel development and debugging. 

### Containers
To ensure reproducibility of results and software, a default docker file is included with this template repository. The respective [README.md](https://github.com/NDCLab/template-tool/blob/main/README.md) contains a comprehensive guide on how to get started with containerization (special thanks to [Jonhas](https://github.com/Jonhas))!

A step-by-step guide to getting started also included in the following [video](https://www.youtube.com/watch?v=oO8n3y23b6M). 

## Workflow
Workflow for both internal and external lab members outlined in the [NDClab contributing wiki doc](https://ndclab.github.io/wiki/docs/contributing.html). 