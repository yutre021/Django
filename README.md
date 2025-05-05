# 🧱 Django Project / Projeto Django

This repository contains a basic Django setup with instructions for development using VS Code.  
Este repositório contém uma configuração básica de Django com instruções para desenvolvimento no VS Code.
Python Version 3.

## 📦 Requirements / Requisitos

- [Python 3.x](https://www.python.org/downloads/)
- [Visual Studio Code](https://code.visualstudio.com/download)
- [Git](https://git-scm.com/downloads)

---

## 🛠️ Setup Guide / Guia de Configuração

### 1. Create and Activate Virtual Environment  
### 1. Criar e Ativar Ambiente Virtual

```bash
# Windows PowerShell
python -m venv venv
.\venv\Scripts\activate
```
```bash
# (If needed)
Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser
```

### 2. Upgrade pip / Atualizar pip
```bash
python -m pip install --upgrade pip setuptools wheel
#See what version is the pip
pip --version

#Upgrade pip
pip install pip --upgrade

#On venv:
python.exe -m pip install --upgrade pip

python -m pip install pip setuptools wheel --upgrade
```

### 🚀 Install Django / Instalar Django
```bash
pip install django
python -m django --version
```

### 📄 Save Requirements / Salvar Dependências
```bash
pip freeze > requirements.txt
```

### Install Requirements / Instalar as dependências
```bash
pip install -r requirements.txt
```

### ⚙️ Create Project and App / Criar Projeto e Aplicativo
```bash
django-admin startproject projeto1 .
cd projeto1
python manage.py startapp app1
python manage.py runserver
```
- Configure `INSTALLED_APPS`, static files, and templates in `settings.py`.
- Configure `INSTALLED_APPS`, arquivos estáticos e templates em `settings.py`.


### 🧪 Testing with Pytest / Testes com Pytest
```bash
pip install pytest
pip install pytest pytest-cov
Ctrl+Shift+P -> Python: Discover Tests
```

### 📂 Project Flow / Fluxo do Projeto

```bash
# Make migrations
python manage.py makemigrations

# Apply migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Enter Django shell
python manage.py shell
```

## 🎨 Templates and Forms

- Create a `templates/` directory
- Use Django Template Language (`{{ variable }}`)
- Handle forms with `GET` and `POST` methods
- Use Bootstrap for styling

### 🌐 Dynamic Pages / Páginas Dinâmicas
- Use query parameters

- Handle form submissions with POST

- Route views using `urls.py` in both project and app


-----------------------------------------------------------------------------------
### Verificar a versão do python (python 3.x.x)

- Criar um ambiente virtaul (python3 -m venv ./env)

- Ativar o ambiente virtual (source ./env/bin/activate)

- Instalação do django (pip install django)

- verificar a versão do djanfo instalada (python -m django --version)

- guardar as dependências (pip freeze > requeriments.txt)
  
-----------------------------------------------------------------------------------

### Criar um projeto Django (django-admin startproject projeto1)

- Fazer as configurações do settings.py (arquivos estáticos e templates)

- Criação de um aplicativo dentro projeto Django (python manage.py startapp app1)

-----------------------------------------------------------------------------------

### criar app "python manage.py startapp app1"

- configuramos as urls (projeto1 e app1)

- criamos uma view (index)

- criamos a pasta de templates

-----------------------------------------------------------------------------------

### criar migrações do model User (python manage.py makemigrations)

- apliquei as migrações (python manage.py migrate)

-----------------------------------------------------------------------------------

- python shell (python manage.py shell) verificação de criação de tabelas

- criar super usuário (python manage.py createsuperuser)

- registrar models no admin.py (app1) 

-----------------------------------------------------------------------------------

### erro na inserção de dados:
  - mudar o campo no models 
  - criar migrações do model User (python manage.py makemigrations)
  - apliquei as migrações (python manage.py migrate)

 - criar templates

-----------------------------------------------------------------------------------

### Criar formulário 

- Testar formulário (GET)

- jinja (engine de templates) -> código no template

- bootstrap (css pré pronto)

-----------------------------------------------------------------------------------

- criação de páginas dinâmicas com método POST

- criação de páginas dinâmicas com query params



### Settings VSCODE
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
    // FOR MAC AND LINUX: "python.defaultInterpreterPath": "venv/bin/python",
    // FOR WINDOWS: "python.defaultInterpreterPath": "venv\\Scripts\\python.exe",
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
