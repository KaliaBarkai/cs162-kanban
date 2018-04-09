All set up should be run from the directory `'.../kanban/'`
# Virtual Env and Installations

command shell:

    python3.6 -m venv .venv
    source .venv/bin/activate
    pip3 install -r requirements.txt

# Set Up Database

python:

    from app import db
    db.create_all()


# Set Up Flask App

command shell:
### For Mac:

    export FLASK_APP=kanban.py
	export FLASK_DEBUG=true
	flask run

### For Windows:

    set FLASK_APP=kanban.py
	set FLASK_DEBUG=true
	flask run

# Run Tests

from directory `'.../kanban/kanban/tests/'`

python

    python tests.py

