# Outline 

* [Roadmap](#Roadmap)  
    * [Overview](#Overview)
    * [Structure](#Directory-Structure)
    * [Function-Standards](#Function-Standards)
* [Containers](#Containers)
* [Git-Workflow](#Git-Workflow)  
* [CI-test](#CI-test)  
* [Reminders](#Reminders)  


## Roadmap

### Overview 

### Directory-Structure
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

## Container
To ensure reproducability of results and software, a default docker file is included with this template repository. The respective [README.md](#container/README.md) contains a comprehensive guide on how to get started with containerization (special thanks to [Jonhas](https://github.com/Jonhas))!

A step-by-step guide to getting started also included in the following [video](https://www.youtube.com/watch?v=oO8n3y23b6M). 

### Function-Standards 


## Containers

## Git-Workflow 

![ndcworkflow](https://user-images.githubusercontent.com/26397102/116148813-00512800-a6a7-11eb-9624-cd81f11d3ada.png)

Development is driven by the [feature branch workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow), where each new feature is encapsulated in a branch. This ensures changes are properly tested & integrated while still allowing for development to be done in parallel.

Subsequently, branches follow this convention:

`main`
- 100% stable and usable by any lab members.
- *No direct commits*

`->dev`
- Up to date development branch with properly tested/reviewed features. 
- *No direct commits*

`-->dev-feature-[featureName]`
- Ongoing development and testing of feature to be pull requested into `dev`.

`--->dev-feature-[featureName]-[yourName]`
- *Only* branch available for personal development, must be branched off of `-->dev-feature-[featureName]` branch.
- Merged into `-->dev-feature-[featureName]` after pull-request.

To ensure branch cleanliness, be sure to enable automatic deletion of branches! To do this hover over to "Settings" and scroll down to the "Automatically delete head branches" option and select the checkbox. 

![image](https://user-images.githubusercontent.com/26397102/123699167-f1b0f980-d82c-11eb-9d6e-b9c24d952401.png)

## CI-test


## Reminders