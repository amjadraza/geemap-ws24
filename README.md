<h1 align="center">
A Template Project for Getting Started with GEEMAP Docker Setup
</h1>

This is a template project to get us started with [geemap](https://geemap.org/) using Docker. Often, it is 
time consuming setting up local python environment to try packages.

Watch below Video

[![alt text](thumbnail.png)](https://youtu.be/Tc5ZJ0RUoS0)

## 🔧 Features
- A template with `poetry` environment
- Jupyter Lab Notebooks
- Running Jupyter Lab in Docker Container
- Running the Jupyter Lab in DevContainer on Vscode

## 💻 Running Locally

1. Clone the repository📂

```bash
git clone https://github.com/amjadraza/geemap-ws24.git
```

2. Install dependencies with [Poetry](https://python-poetry.org/) and activate virtual environment🔨

```bash
poetry install
poetry shell
```

3. Configure Environment Variables

given `.env.example`, rename to `.env` and replace the desired Environment Variable

```bash

jupyter lab
```

4. Run the Jupyter Lab server🚀

```bash

jupyter lab
```
Explore the sampled notebooks with sample data

## Running in local Docker Container

When creating envronments, we often face lot of dependency and frameworks issues and it consumes lot of 
our time in figuring out these issues. Docker setup is useful in solving these issues. 

To run the application Docker, use

```docker-compose up```

> Make sure Docker Desktop is installed on Windows Machine or Docker on Mac and Ubuntu

## Running in Project in DevContainer with VsCode

If you are using Vscode as your preffered IDE, it comes with Development Container Setup which creates a development environment in isolation by starting a container as if you are working on your local machine.

Read More on : https://code.visualstudio.com/docs/devcontainers/devcontainer-cli

Steps:

1. Install DevContainer Extension
2. You will see `.devcontainer.json` file with settings
3. On your left-bottom, see the arrows sysmbole
4. Click, a dialoge with Remote Development Environemnet will pop up
5. Select `Reopen in Container`, It will create a docker container first time.
6. Thats all you are up & running

Run below command to start a Jupyter Notebook in your DevContainer Environement

```jupyter lab --ip='0.0.0.0' --port=8888 --no-browser --allow-root```


## Credits / Resources

1. [Geemap Resource](https://geemap.org/workshops/SatMOC_2024/)


