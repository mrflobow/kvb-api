kvb-api
=======

## Installation

	python3 -m venv env
	source env/bin/activate
	pip install beautifulsoup4 requests flask
	pip install parse
	pip install werkzeug==0.16.0

## PI Guide

    sudo apt install python3-pip 
    mkdir ~/kvbapi
    cd ~/kvbapi
    git clone https://github.com/KoelnAPI/kvb-api.git .
    python3 -m venv env
	source env/bin/activate
    pip install beautifulsoup4 requests flask
    pip install wheel
    pip install parse
    pip install werkzeug==0.16.0
    deactivate


Copy systemd file to service

    sudo cp kvbapi.service /etc/systemd/system/kvbapi.service
    sudo systemctl enable kvbapi.service
    sudo systemctl start kvbapi.service


## Start

    python server.py



Ein paar Test-URLs:

    http://127.0.0.1:6000/
    http://127.0.0.1:6000/stations/
    http://127.0.0.1:6000/stations/1/
    http://127.0.0.1:6000/stations/2/
    http://127.0.0.1:6000/stations/3/
