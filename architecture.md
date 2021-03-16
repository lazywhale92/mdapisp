# Project description

## Execution environment
* written and tested in Python 3.7.3 (via pyenv virtual environment)
* if you are using pip as your package manager : plz check, requirements.txt 
* if you are using poetry as your package manager : plz check, pyproject.toml and poetry.lock 

##  architecture design & the reason for design
* Focused on __minimum difficulty and minimum cost implementation__ to meet the requirements specification.
    * only the logic for the api was written without implementing a web server (ex. nginx, apache, etc.), the database also used __sqlite__, and it was written as lightly as possible using __fastapi__ to avoid swegger implementation.



## How to run
* Basically, start.sh has been prepared according to the requirements, so you can run start.sh, but if a problem occurs, run it as follows.

1. Copy `mdapisp_0.0.0-py3-none-any.whl` to a suitable directory

1. Run `!pip uninstall mdapisp -y && pip install mdapisp-0.0.0-py3-none-any.whl`

1. Run `uvicorn main:app --reload`

1. If you want to enter the testable Swagger page with the GUI, you can access localhost:port/doc#.
Basically http://127.0.0.1:8000/docs#/
