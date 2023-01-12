# Links
Abaixo estão todos os links mencionados na aula:

- VS Code: https://code.visualstudio.com/download
- Chrome: https://www.google.com/intl/pt-BR/chrome/
- Python: https://www.python.org/downloads/
- Git: https://git-scm.com/downloads

## Powershell
Não se esqueça de configurar o powershell com o comando abaixo (como administrador):

```
Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser

```

## Create the project directory
mkdir tutorial
cd tutorial

## Create a virtual environment to isolate our package dependencies locally
python3 -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`

## Install Django and Django REST framework into the virtual environment
pip install django
pip install djangorestframework

## Configuração do VS Code para Python e Django.
```
settings.json

{
  "window.zoomLevel": 0,
  "python.languageServer": "Pylance", // ms-python.vscode-pylance
  "python.testing.unittestEnabled": false, // ms-python.python
  "python.testing.pytestEnabled": true,
  "python.testing.pytestArgs": [], // -x to bail
  "python.linting.flake8Enabled": true,
  "python.linting.mypyEnabled": true,
  "python.linting.pylintArgs": [
    "--load-plugins=pylint_django",
    "--errors-only"
  ],
  "python.formatting.autopep8Args": ["--indent-size=4"],
  "python.defaultInterpreterPath": "venv/bin/python",
  "[python]": {
    "editor.defaultFormatter": "ms-python.python", // ms-python.python
    "editor.tabSize": 4,
    "editor.insertSpaces": true,
    "editor.formatOnSave": true,
    "editor.formatOnType": true,
    "editor.codeActionsOnSave": {
      "source.organizeImports": true
    }
  },
  "[html]": {
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "vscode.html-language-features",
    "editor.quickSuggestions": {
      "other": true,
      "comments": true,
      "strings": true
    }
  },
  "[django-html]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": "vscode.html-language-features",
    "editor.quickSuggestions": {
      "other": true,
      "comments": true,
      "strings": true
    }
  },
  "files.associations": {
    "*.js": "javascript",
    "*.jsx": "javascriptreact",
    "*.xml": "html",
    "*.svg": "html",
    "*.html": "html",
    "django-html": "html", // batisteo.vscode-django
    "**/*.html": "html",
    "**/templates/**/*.html": "django-html",
    "**/base_templates/**/*.html": "django-html",
    "**/requirements{/**,*}.{txt,in}": "pip-requirements"
  },
  "emmet.includeLanguages": {
    "django-html": "html", // batisteo.vscode-django
    "javascript": "javascriptreact",
    "typescript": "typescriptreact"
  }
}
```
## Instalar dependencias com o requirements.txt
pip install -r requirements.txt
