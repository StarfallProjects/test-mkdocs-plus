## Prerequisites

* git installed on your machine
* A GitHub account
* A terminal. This tutorial used PowerShell 7.2. If you are on Linux or macOS, some commands will be different.
* A text editor

## Create a repo

1. Open a terminal, navigat into you site's directory, and activate your virtual environment.
2. Create a .gitignore:
    ```shell
    ni .gitignore
    ```
3. Open your `.gitignore` and add the following:
    ```txt
    venv
    node_modules
    site
    ```
4. Create a local repo:
    ```shell
    git init
    ```
5. Go to GitHub and create a new repository. Don't add a README or .gitignore.
6. Work through these commands to connect your local repo to the GitHub repo:
    ```shell
    git remote add origin https://github.com/<YourGitHubName>/<your-repo-name>.git
    git branch -M main
    git add --all
    git commit -m "first commit"
    git push -u origin main
    ```
    Depending on how git is configured, you may be prompted to log in during the process.