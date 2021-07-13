# Python + Docker: Python-env evolution [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

## :clipboard: Introduction

Developing Python projects in local environments can get pretty challenging if more than one project is being developed at the same time. Bootstrapping a project may take time as we need to manage versions, set up dependencies and configurations for it. Before, we used to install all project requirements directly in our local environment and then focus on writing the code. But having several projects in progress in the same environment becomes quickly a problem as we may get into configuration or dependency conflicts. Moreover, when sharing a project with teammates we would need to also coordinate our environments. For this we have to define our project environment in such a way that makes it easily shareable. 

A good way to do this is to create isolated development environments for each project.

## :cloud: Getting Started

Follow along this notes. You will need to have at least [Docker](https://www.docker.com/) installed and [VSCode](https://code.visualstudio.com/) to edit files project (Include some plugins to easy more develop). 

You can use some package management tool for windows. E.g. [Chocolatey](https://chocolatey.org/)

*	[Docker Windows](https://www.docker.com) - Application virtualizer

```
choco install docker-desktop -y
```

*	[Visual Studio Code](https://code.visualstudio.com/) - Integrated Development Environment (IDE) + plugins

```
choco install vscode -y
choco install vscode-docker -y
choco install vscode-python -y
```

Clone this repository, and fire up a command-line tool.

## :computer: Steps

To execute the next command line:

```
docker build -t hello-word-service-image -f Dockerfile-slim .
docker run -d -p 5000:5000 --name hello-word-service hello-word-service-image
```

And check exposed service:

```
curl http://localhost:5000
```

## :octocat: Can you support me?

I will continue to do things and expose notes, but existing many ways to support what I do:
* Pull requests are welcome a :dizzy:
* Don't forget to give this Repository a :star2:
* <a href="https://www.buymeacoffee.com/pedringcoding" title="Donate to this content using BuyMeACoffee">Buy me a :coffee:</a>