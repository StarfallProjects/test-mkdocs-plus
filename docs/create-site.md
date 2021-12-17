## Prerequisites

* Python 3.x and pip. This tutorial was created using Python 3.10.
* A terminal. This tutorial used PowerShell 7.2. If you are on Linux or macOS, some commands will be different.
* A text editor.

## Create the site

1. In your terminal, create an empty directory and `cd` into it:
    ```shell
    mkdir example-site
    cd example-site
    ```
2. Create a virtual environment and activate it:
    ```shell
    python -m venv venv
    .\venv\scripts\activate.ps1
    ```
    You will need to activate the environment evert time you start a new terminal session.
3. Install Material Insiders. Refer to the [Material Insiders installation guide](https://squidfunk.github.io/mkdocs-material/insiders/getting-started/) for details.
    ```shell
    pip install git+https://${GH_TOKEN}@github.com/squidfunk/mkdocs-material-insiders.git
    ```
4. Create a new MkDocs site:
    ```shell
    mkdocs new .
    ```
5. Open `mkdocs.yml` and set the theme:
    ```yaml
    theme:
      name: material
    ```
    Refer to [Material - Creating your site](https://squidfunk.github.io/mkdocs-material/creating-your-site/) for guidance on other configuration settings.
6. Check everything has worked by serving the site locally:
    ```shell
    mkdocs serve
    ```
