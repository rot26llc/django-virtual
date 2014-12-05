django-virtual
==============

django in a virtual environment

# Requirements

1) Python
2) Python virtualenv
    - ![virtualenv documentation][venv_doc]

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

directory structure (2 levels)
```
.env
├── bin
│   ├── activate
│   ├── activate.csh
│   ├── activate.fish
│   ├── activate_this.py
│   ├── easy_install
│   ├── easy_install-3.4
│   ├── pip
│   ├── pip3
│   ├── pip3.4
│   ├── python -> python3.4
│   ├── python3 -> python3.4
│   └── python3.4
├── include
│   └── python3.4m -> /usr/local/Cellar/python3/3.4.2_1/Frameworks/Python.framework/Versions/3.4/include/python3.4m
└── lib
    └── python3.4
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
```?

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
