# Python Pattern References

clone the repo:

    florian@florian-desktop ~/ws_github/python-pattern-language $ git clone https://github.com/python-pattern-language/python-pattern-references.git

create a clean virtual environment (venv):

    florian@florian-desktop ~/ws_github/python-pattern-language $ cd python-pattern-language
    florian@florian-desktop ~/ws_github/python-pattern-language $ virtualenv -p /usr/bin/python3.4 --no-site-packages venv

activate the venv and check it:

    florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ source venv/bin/activate
    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ pip freeze
    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ python --version
    Python 3.4.3

install sphinx:

    pip install sphinx

save the venv dependencies into a requirement file:

    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ pip freeze > venv/requirements.txt

setup the documentation sources with the following options:

    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ sphinx-quickstart
    ...
    > Root path for the documentation [.]:
    ...
    > Separate source and build directories (y/n) [n]:
    ...
    > Name prefix for templates and static dir [_]:
    ...
    > Project name: Python Pattern References
    > Author name(s): Florian Kromer
    ...
    > Project version: 0.1
    > Project release [0.1]:
    ...
    > Project language [en]:
    ...
    > Source file suffix [.rst]:
    ...
    > Name of your master document (without suffix) [index]:
    ...
    > Do you want to use the epub builder (y/n) [n]:
    ...
    > autodoc: automatically insert docstrings from modules (y/n) [n]: 
    > doctest: automatically test code snippets in doctest blocks (y/n) [n]: 
    > intersphinx: link between Sphinx documentation of different projects (y/n) [n]: 
    > todo: write "todo" entries that can be shown or hidden on build (y/n) [n]: 
    > coverage: checks for documentation coverage (y/n) [n]: 
    > imgmath: include math, rendered as PNG or SVG images (y/n) [n]: 
    > mathjax: include math, rendered in the browser by MathJax (y/n) [n]: 
    > ifconfig: conditional inclusion of content based on config values (y/n) [n]: 
    > viewcode: include links to the source code of documented Python objects (y/n) [n]: 
    > githubpages: create .nojekyll file to publish the document on GitHub pages (y/n) [n]:
    ...
    > Create Makefile? (y/n) [y]: 
    > Create Windows command file? (y/n) [y]:
    
    Creating file ./conf.py.
    Creating file ./index.rst.
    Creating file ./Makefile.
    Creating file ./make.bat.
    
    Finished: An initial directory structure has been created.

install the sphinx-doc theme "read the docs" and update the requirements:

    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ pip install sphinx_rtd_theme
    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ pip freeze > venv/requirements.txt

adjust the configure to the new theme in conf.py ("html_theme =")

generate the html files:

    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ make html

add content...
