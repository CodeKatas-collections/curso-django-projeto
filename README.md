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
