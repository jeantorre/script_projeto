poetry add black flake8 isort pre-commit mkdocs mkdocs-material mkdocstrings-python taskipy pytest ignr

pre-commit: - poetry run pre-commit install  
mkdocs: - poetry run mkdocs new .  
ignr: - poetry run ignr -p python > .gitignore  
