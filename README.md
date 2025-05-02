# Django
Here i gonna show my working on Django

Python Version 3.

-VS Code: https://code.visualstudio.com/download

-Python: https://www.python.org/downloads/

-Git: https://git-scm.com/downloads

Create new folder on Vs Code


Open the terminal

"python -m venv venv"

Activate type on terminal: .\venv\Scripts\activate


Waning: Use  carefully on Powershell
Não se esqueça de configurar o powershell com o comando abaixo (como administrador):

Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser


See what version is the pip (pip --version)

Upgrade pip (pip install pip --upgrade)

On venv: python.exe -m pip install --upgrade pip

pip install pytest
pip install pytest pytest-cov
Ctrl+Shift+P -> Python: Discover Tests


python -m pip install pip setuptools wheel --upgrade


-----------------------------------------------------------------------------------
Verificar a versão do python (python 3.x.x)

Criar um ambiente virtaul (python3 -m venv ./env)

Ativar o ambiente virtual (source ./env/bin/activate)

Instalação do django (pip install django)

verificar a versão do djanfo instalada (python -m django --version)

guardar as dependências (pip freeze > requeriments.txt)
-----------------------------------------------------------------------------------

Criar um projeto Django (django-admin startproject projeto1)

Fazer as configurações do settings.py (arquivos estáticos e templates)

Criação de um aplicativo dentro projeto Django (python manage.py startapp app1)

-----------------------------------------------------------------------------------

criar app "python manage.py startapp app1"

configuramos as urls (projeto1 e app1)

criamos uma view (index)

criamos a pasta de templates

-----------------------------------------------------------------------------------

criar migrações do model User (python manage.py makemigrations)

apliquei as migrações (python manage.py migrate)

-----------------------------------------------------------------------------------

python shell (python manage.py shell) verificação de criação de tabelas

criar super usuário (python manage.py createsuperuser)

registrar models no admin.py (app1) 

-----------------------------------------------------------------------------------

erro na inserção de dados:
  mudar o campo no models 
  criar migrações do model User (python manage.py makemigrations)
  apliquei as migrações (python manage.py migrate)

criar templates

-----------------------------------------------------------------------------------

Criar formulário 

Testar formulário (GET)

jinja (engine de templates) -> código no template

bootstrap (css pré pronto)

-----------------------------------------------------------------------------------

criação de páginas dinâmicas com método POST

criação de páginas dinâmicas com query params



settings vscode
```json
{
    "window.zoomLevel": 0,
    "editor.fontSize": 19,
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
    // "python.defaultInterpreterPath": "venv/bin/python",
    "[python]": {
      "editor.defaultFormatter": "ms-python.python", // ms-python.python
      "editor.tabSize": 4,
      "editor.insertSpaces": true,
      "editor.formatOnSave": true,
      "editor.formatOnType": true,
      "editor.codeActionsOnSave": {
        "source.organizeImports": "explicit"
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
