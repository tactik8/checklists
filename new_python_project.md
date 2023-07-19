
# Checklist: New Python Project
Date created: 2023-07-19
Date updated: 2023-07-19


# Overview
Checklist of activities ot create a new python project, store it in github and publish on pypi as library or on google app as application

# Activities

## Setup
### in repl.it
- Create new project in repl.it
- Copy files from /new_python_project in main directory of repl.it
- Update areas with < > in setup.py
- Update readme.md
- Create .gitignore file in main directory on repl.it with following content:
  - poetry.lock
  - pyproject.toml
  - .pytest_cache
  - .replit
  - replit.nix
  - .upm


### in github
#### if creating a pypl library:
- create action from template "Publish Python Package"
- create new security token in pypi
- add security token as environment variable under settings - secrets and variables - actions, name PYPI_API_TOKEN

#### if publishing to google app
- in google app, setup new trigger


## Execution

### Deploying new pypi library
#### In repl.it:
- Increment setup.py version number
- In github, create new release using same version no
- github actions will automatically publish to pypi


