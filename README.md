# Scaffold a Flask Project

This article details how to build a scaffolding tool used to generate a Flask boilerplate.

Blog post: https://realpython.com/blog/python/scaffold-a-flask-project/

## TLDR
If you want a clean virtualenv in the template, do the following,
otherwise, you can skip this part to use your system python and
packages.
```bash
$ pip install virtualenv
$ cd flask_scaffold
$ rm -rf env requirements.txt
$ python -m venv env
$ source env/bin/activate
$ pip install jinja2
$ pip freeze > requirements.txt
```

Generate a new project
```bash
$ python flask_skeleton.py new_project -s skeleton -b 'angular, jquery, bootstrap' -g -v
```

Run the management server
```bash
$ python manage.py runserver --host=0.0.0.0 --port=6011
```
