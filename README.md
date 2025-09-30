# Why a project template?

This project is a starter template for new student
projects with Andreas Paepcke. It sets up a file 
structure with a few files that illustrate style
and some Python/Unittest facilities.

The template contains a small example project that
pretends to predict ancient Greek professions from 
names.

Features that are demonstrated are:

    o Class/method setup
    o Unit testing in an object-oriented context
    o Argparse
    o Creation of executable script using #!
    o Use of pyproject.toml

# Creating new project from this template

Usually Andreas will pre-create a Github repo for you, and
it will contain a sample setup in which you replace pyproject.toml,
README.md, and Python packages/modules under <proj-root>src.

But to create your own repo based on this project template, proceed
as follows:

    o Create your own repo on github, and note its clone URL,
        say git@github.com:john_doe/your_project.git
    o On your machine, clone this project_template:
        `git clone git@github.com:paepcke/project_template.git`
    o cd project_template
    o git push --mirror git@github.com:john_doe/your_project.git
    o cd ..
    o git clone git@github.com:john_doe/your_project.git
    o cd your_project

Change to your <proj-root>.
    
# Setup and install the example

Naming conventions: a Python 'package' is a directory that includes
a (possibly empty) file called `__init__.py`. A 'module' is a Python
file inside a package directory.

After cloning, 
    
    o cd your_project
    o Edit pyproject.toml to match your name, project name, etc.
    o Optionally create an anaconda environment (highly recommended)
         conda new -s your_project

In the `<proj-root>/src` you will find a fake application, which you
replace with your own Python code. Of course, rename the package
`greeknames` to your own package name, and feel free to add additional
packages.

Update the `pyproject.toml` file whenever you require another package
from PyPi. Then:

```
pip install .
```
  


