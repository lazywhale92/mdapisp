# Project description

## Execution environment
* written and tested in Python 3.7.3 (via pyenv virtual environment)
* if you are using pip as your package manager : plz check, requirements.txt 
* if you are using poetry as your package manager : plz check, pyproject.toml and poetry.lock 

##  architecture design & the reason for design
* Focused on __minimum difficulty and minimum cost implementation__ to meet the requirements specification.
    * only the logic for the api was written without implementing a web server (ex. nginx, apache, etc.), the database also used __sqlite__, and it was written as lightly as possible using __fastapi__ to avoid swegger implementation.
