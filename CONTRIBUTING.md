# Outline 

* [Roadmap](#Roadmap)  
    * [Overview](#Overview)
    * [Structure](#Directory-Structure)
    * [Function-Standards](#Function-Standards)
* [Containers](#Containers)
* [Git-Workflow](#Git-Workflow)  
* [CI-test](#CI-test)  
* [Output-Data](#Output-Data)
* [Reminders](#Reminders)  


## Roadmap

### Overview 

### Directory-Structure
```yml
baseEEG
├── run.py
├── scripts
|    ├──__init__.py
|    ├──package1
|    |    ├──__init__.py
|    ├──package2
|    |    ├──__init__.py
```

### Function-Standards 


## Containers

## Git-Workflow 

![ndcworkflow](https://user-images.githubusercontent.com/26397102/116148813-00512800-a6a7-11eb-9624-cd81f11d3ada.png)

Development is driven by the [feature branch workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow), where each new feature is encapsulated in a branch. This ensures changes are properly tested & integrated while still allowing for development to be done in parallel.

Subsequently, branches follow this convention:

`main`
- No test features
- 100% stable and usable by any lab members 
- *No direct commits*

`->dev`
- Up to date development branch with properly tested/reviewed features 
- *No direct commits*

`-->dev-feature-[featureName]`
- Ongoing development and testing of feature to be pull requested into `dev` 
- *No direct commits*

`--->dev-feature-[featureName]-[yourName]`
- *Only* branch available for personal development, must be branched off of `-->dev-feature-[featureName]` branch
- Merged into `-->dev-feature-[featureName]` after pull-request (code review)


## CI-test


## Example-Data


## Reminders
