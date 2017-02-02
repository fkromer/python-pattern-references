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

install mkdocs:

    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ pip install mkdocs

save the venv dependencies into a requirement file:

    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ pip freeze > venv/requirements.txt

host the website on locally:

    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ mkdocs serve

add content... (local server shows updated version on-the-fly)

add and commit chagnes to master branch:

    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ git add ...
    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ git commit ...

deploy to gh-pages branch:

    (venv)florian@florian-desktop ~/ws_github/python-pattern-language/python-pattern-references $ mkdocs deploy gh-pages

visit [Python Pattern References Website](https://fkromer.github.io/python-pattern-references/) hosted with GitHub Pages
