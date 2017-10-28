# Python Pattern References

clone the repo:

    git clone https://github.com/python-pattern-language/python-pattern-references.git

create a clean virtual environment (venv):

    cd python-pattern-language
    virtualenv -p /usr/bin/python3.4 --no-site-packages venv

activate the venv and check it:

    source venv/bin/activate
    (venv) pip freeze
    (venv) python --version
    Python 3.4.3

install mkdocs:

    (venv) pip install mkdocs

save the venv dependencies into a requirement file:

    (venv) pip freeze > venv/requirements.txt

host the website on locally:

    (venv) mkdocs serve

add content... (local server shows updated version on-the-fly)

add and commit chagnes to master branch:

    (venv) git add ...
    (venv) git commit ...

deploy to gh-pages branch:

    (venv) mkdocs deploy gh-pages

visit [Python Pattern References Website](https://fkromer.github.io/python-pattern-references/) hosted with GitHub Pages
