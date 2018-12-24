# Quality TP-2 Compte Rendu
By **SAMET MohamedAmin** and **DGHAIES Ahmed** GL4/2

## Description
This assignmint is a step-by-step description of a docker-compose application tailed with a demonstration of kubernetes. This application covers most of the tools described in the workshop.

## Environment
- linux os: Fedora 29
- Windows os: Windows 10
- Docker: 18.06.1-ce
- Kubernetes
  - client: v1.10.3
  - server: v1.10.0
- minkube: v0.30.0
- Jenkins: 2.152
  - Pipeline: 2.6
  - Build Pipeline Plugin: 1.5.8	
  - Checkstyle Plug-in: 4.0.0	
  - Copy Artifact Plugin: 1.41	
  - Deploy to container Plugin: 1.13
  - JIRA plugin: 3.0.5
  - Kubernetes: 1.14.0	
- SonarQube: 6.7.6
- tomcat: 8.5 lts
- mongo: 4.0.4 lts
- Jira: 7.13


## Content
- [tools description](tools_description.md)
  - [Docker](tools_description.md#docker)
    - [Docker setup](tools_description.md#docker_setup)
      - [Installation](tools_description.md#installation)
      - [Run service](tools_description.md#run-service)
      - [Demonstration](tools_description.md#Demonstration)
  - [Sonarqube](tools_description.md#sonarqube)
    - [Sonarqube structure](tools_description.md#sonarqube_structure)
    - [Sonarqube test](tools_description.md#sonarqube_test)
  - [Jenkins](tools_description.md#jenkins)
    - [Jenkins setup](tools_description.md#jenkins_setup)
    - [New project](tools_description.md#new_project)
- [main application](main_app.md)
  - [Structure](main_app.md#structure)
  - [Jenkins](main_app.md#jenkins)
    - [Global tool configuration](main_app.md#global-tool-configuration)
    - [Plugins](main_app.md#plugins)
    - [starting new project](main_app.md#starting-new-project)
  - [Checkstyle](main_app.md#checkstyle)
  - [Tomcat](main_app.md#tomcat)
  - [Sonarqube](main_app.md#sonarqube)
- [jenkins pipeline](jenkins_pipeline.md)
  - [Why the use of pipeline](jenkins_pipeline.md#why-the-use-of-pipeline)
  - [Pipeline process](jenkins_pipeline.md#pipeline-process)
- [kubernetes demo](kubernetes.md)
  - [Introduction](kubernetes.md#introduction)
  - [Setup](kubernetes.md#setup)
  - [Understanding kubernetes basics](kubernetes.md#understanding-kubernetes-basics)
    - [First step](kubernetes.md#first-step)
    - [Loading configuration](kubernetes.md#loading-configuration)
    - [Understanding minikube concept](kubernetes.md#understanding-minikube-concept)
    - [Deleting loaded configuration](kubernetes.md#deleting-loaded-configuration)
  - [Deployment object](kubernetes.md#deployment-object)
  - [Dashboard](kubernetes.md#dashboard)
  - [Jenkins Kubernetes plugin](kubernetes.md#jenkins-kubernetes-plugin)
- [jira](jira.md)
  - [Basic use](jira.md#basic-use)
  - [Jenkins Integration](jira.md#jenkins_integration)

## TODO
- [x] docker explaination
- [x] kubernetes example
- [x] explain pipeline build in details
- [x] fully integegrate madou's part
- [x] jenkins description
- [x] jira plugin
- [x] add checkstyle demo
- [x] seperate the project paragraphs
- [x] add tools versions
- [ ] check globally the assignment