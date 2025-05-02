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

Powershell
Não se esqueça de configurar o powershell com o comando abaixo (como administrador):

Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser

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
