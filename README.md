# PySeas - Open Source Pirate (Adventure) Board Game

[![Discord](https://discord.com/api/guilds/1272287320934056066/widget.png)](https://discord.gg/s2P9fZbeZs)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://www.freecodecamp.org/news/how-to-make-your-first-pull-request-on-github-3/)
[![License](https://img.shields.io/github/license/ultimateownsz/pyseas)](https://github.com/ultimateownsz/PySeas/blob/main/LICENSE)

<img src="https://i.postimg.cc/NM5R3tzW/100x100-map.png" />


## Project Description

PySeas is a community-driven project to create an exciting and engaging pirate themed adventure board game inspired by the game Sea of Thieves. This game is designed to be engaging and using interactive elements using tools called Python and Pygame-CE, but you don't need to be a programmer to get involved or enjoy it!


## Why Join PySeas?

- **Increasing your skills**: Learn and improve your Python and Pygame skills through practical, hands-on development.
- **Learn about game development**: Explore the world of game development and design, gaining valuable experience along the way.
- **Create something enjoyable**: Contributing to a project that results in a game you and others can enjoy.
- **Join our community on [Discord](https://discord.gg/MZ5MHqDnGW)**: Whether you want to help with ideas, give feedback, or simply enjoy the game, everyone is welcome!


## Getting started

No need to worry if you are new to programming. This guide will walk you through the setup step by step. by the end, you'll have everything ready to run the Pyseas project.


1. **Clone the Repository:**
First you'll need to copy the Pyseas project to your computer through a process called "cloning".
```
  git clone https://github.com/ultimateownsz/pyseas.git
```

2. **Set up a virtual environment:** 
A virtual environment is like a seperate space on your computer where you can install the software needed for this project without affecting other programs.
- **For Mac or Linux Users:**
  1. In your terminal, navigate to the folder where you downloaded the project (usually the 'pyseas' folder) using the 'cd' command:
    ```bash
    cd pyseas
    ```
  2. Set up the virtual environment by typing: 
    ```bash
    python3 -m venv venv
    ```
  3. Activate the virtual environment:
     ```bash
     source venv/bin/activate
     ```

- **For Windows Users**:
    1. Open Command Prompt and navigate to the 'pyseas' folder (where you downloaded the project) using the 'cd' command:
    ```bash
    cd pyseas
    ```
    2. Set up the virtual environment by typing:
    ```bash
    python3 -m venv venv
    ```
    3. Activate the virtual environment:
    ```bash
    venv\Scripts\activate
    ```
  
3. **Install Required Software**:
Now, you'll need to install the necessary software that the project depends on.
  1. Make sure you're still in the 'pyseas' directory/folder and that the virtual environment is active.
  2. Install the software by typing the following command:
  ```
  pip install -r requirements.txt # For running the game (runtime dependencies)
  ```
This installs everything you need to run the project.
  3. If you plan to do any local development or modifications, also run:
  ```
  pip install -r requirements_dev.txt # For local development
  ```

This step is optional and only needed if you want to make changes to the project.
4. **Run the project**
Now you are ready to start the project!
  1. Simply type:
  ```
  python main.py
  ```
  2. The project should start running, and you'll see it in action!

**Deactivate the Virtual Environment**:
When you’re done working, you can deactivate the virtual environment using:
```bash
deactivate
```

## Reporting bugs & requesting features
If you find something that's not working right or have an idea to make our project better, you can let us know by opening an `Issue` here on [Github](https://github.com/ultimateownsz/PySeas/issues). An issue is just a way to tell us about a problem or suggest a new feature.

We use [Github_Projects](https://github.com/users/ultimateownsz/projects/5) to organize and keep track of these issues, so we can make sure everything gets the attention it needs.

If you need more help or want to talk about it, you can join our [Discord](https://discord.gg/MZ5MHqDnGW) community. We're here to chat and help you out!


## Local Development
**See how to contribute:** [contribute](./CONTRIBUTING.md)

### Linting and Formatting for developers
We chose to use [Ruff](https://docs.astral.sh/ruff/) to automatically lint and format the code. `Run pip install -r requirements_dev.txt` to install Ruff and other relevant dependencies.

> [!IMPORTANT]
> **Before you open a Pull Request, please run this bash commands to format your code properly and doesn't upset our linter:**
>
> 
> ```sh
> ruff format . && ruff check --include I --fix . # this formats code and sort imports
> ruff check . # run linting and perform fixes
> mypy main.py
> ```
>
> **If you use powershell, run these commands:**
>
> ```powershell
> ruff format .;
> ruff check --include I --fix .;
> ruff check .;
> mypy main.py
> ```
