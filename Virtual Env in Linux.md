### <span style="color:blue"> **Before You Begin:**</span>

1. Update your system:
```
    sudo apt-get update && sudo apt-get upgrade
```

2. Install the virtualenv tool using your package manager:
```
    sudo apt install virtualenv
```


### <span style="color:blue">**Create a Python Virtual Environment:**</span>

1. Create a python-environments directory in your user’s home directory and navigate to it:
```
    mkdir ~/python-environments && cd ~/python-environments
```

2. Create a Python virtual environment. By default, virtualenv attempts to use the Python 2.5 interpreter to create a new environment. Since Ubuntu 18.04 does not have Python 2 installed, you should use the --python option to tell virtualenv to use your system’s Python 3.6 interpreter. Replace env with the name you would like to assign to your virtual environment.
```
    virtualenv --python=python3 env
```

3. Validate that your environment is installed with the version of Python that you expect:
```
    ls env/lib
```


### <span style="color:blue">**Activate Your Virtual Environment:** </span>

1. Activate the newly created virtual environment:
```
    source env/bin/activate
```

### <span style="color:blue">**Dectivate a Virtual Environment:** </span>

1. To deactivate an active virtual environment, issue the following command:
```
    deactivate
```