poetry add --group dev black flake8 isort pre-commit mkdocs mkdocs-material mkdocstrings-python taskipy pytest ignr

pre-commit: - poetry run pre-commit install  
mkdocs: - poetry run mkdocs new .  
ignr: - poetry run ignr -p python > .gitignore  

# Instalar todas as bibliotecas de (desenvolvimento e principais)
poetry install --with dev --no-root

# Instalar apenas as bibliotecas principais
poetry install --only main --no-root
