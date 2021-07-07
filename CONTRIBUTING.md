# Contributing to [project name]

## Overview
Please note our general guidelines for contributing to NDCLab projects [here](https://ndclab.github.io/wiki/docs/contributing.html).

* [Roadmap](#Roadmap)  
* [Directory-Structure](#Directory-Structure)  
* [Scripts](#Scripts)
* [Containers](#Containers)  
* [Workflow](#Workflow)  

## Roadmap
Please see the roadmap available on the README.md file of this repository.

## Directory-Structure
```yml
baseEEG
├── run.py
├── scripts
|    ├──__init__.py
├── container
|    ├──Dockerfile.template 
|    ├──environment.yml
|    ├──README.md 
├── .github 
```

## Scripts
The `scripts` directory is where Python modules will be pulled from. This ensures that modules are neatly divided according to responsibility, which helps with parallel development and debugging. 

More info on creating packages [here](https://docs.python.org/3/tutorial/modules.html#packages). 

## Containers
To ensure reproducability of results and software, a default docker file is included with this template repository. The respective [README.md](#container/README.md) contains a comprehensive guide on how to get started with containerization (special thanks to [Jonhas](https://github.com/Jonhas))!

A step-by-step guide to getting started also included in the following [video](https://www.youtube.com/watch?v=oO8n3y23b6M). 

## Workflow
Workflow for both internal and external lab members outlined in the [NDClab contributing wiki doc](https://ndclab.github.io/wiki/docs/contributing.html). 