# Handbook development

Technogi's Handbook uses [MkDocs] that's geared towards building project documentation. Documentation source files are written in Markdown, and configured with a single YAML configuration file. Start by reading the introduction below, then check the [User Guide](https://www.mkdocs.org/user-guide/writing-your-docs/) for more info.

## Environment setup

In order to start development on Technogi's Handbook, a [Python] version of at least 3.5 is required and a [pip] version of at least 18.0. 

First, clone the repository:

``` bash
git clone https://github.com/Technogi/handbook
```

Next, all dependencies need to be installed, which is done with:

``` bash
cd handbook
pip install -r requirements.txt
```

## Development mode

Start the MkDocs server with:

``` bash
mkdocs serve
```

Point your browser to [localhost:8000][1] and you should see the handbook in front of you.

> *__"Automatically generated files"__*
Never make any changes in the `site` directory, as the contents of this
directory are automatically generated from the `docs` directory and will be
overridden when the handbook is built.

  [1]: http://localhost:8000

## Build process

When you've finished making your changes, you can build the handbook by invoking:

``` bash
mkdocs build
```

This triggers the production-level compilation and minification of all
stylesheets and JavaScript sources. When the command exits, the final files are
located in the `site` directory.

Now you can see the handbook with your changes to the original.

[MkDocs]: https://www.mkdocs.org/
[pip]: https://pip.readthedocs.io/en/stable/installing/
[Python]: https://www.python.org/