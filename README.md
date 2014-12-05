django-virtual
==============

django in a virtual environment

# Requirements

1) Python

2) Python virtualenv
* ![virtualenv documentation][venv_doc]

# Virtual Environment

Uses Python virtualenv


1) Install Python virtualenv on local machine

```sh
$ pip install virtualenv
```

2) Create a virtual python environment

```sh
$ virtualenv .env
```

3) Activate the Virtual Environment

```sh
$ source ./.env/bin/activate
(.env)$ 
```

4) Install packages with pip

```sh
(.env)$ pip install -r pip_freeze
```

5) Do your work

```sh
vim .
```

6) Freeze packages if you have added any

```sh
(.env)$ pip freeze > pip_freeze
```

7) deactivate the python virtual environment

```sh
(.env)$ deactivate
$ 
```

8) Repeat steps 3 through 7 as necessary

[venv_doc]: http://virtualenv.readthedocs.org/en/latest/virtualenv.html
