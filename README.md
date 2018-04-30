# Flask Template

## What is this 

Flask leaves the organization of your application up to you. This is one of the reasons why I liked it, but it does mean that you have to put some thought into how to structure your code. You could put your entire application in one file, or have it spread across multiple packages.

There are a few organizational patterns that you can follow to make development and deployment easier. And this is my way.

## How to use it?

1. Firstly, clone it via: `git clone https://github.com/GreatBahram/Flask-Template`

2. All requirements are written in `requirements.txt` file. So, you should create `Virtualenv` then install those requirements (`pip3 install -r requirements.txt`).
3. I've Created Class-based configuration file in `config.py`.  There are three main class: `development`, `production` and `testing`. To determine which configuration you want to use, do that via `export FLASK_CONFIG="development"` for example.
4. Run the project. You can do that yourself via `python3 run.py` or let's flask do that for you with `export   FLASK_APP=run.py && flask run`.

### Files Structure

```sh
Flask-Template
├── app
│   ├── __init__.py
│   ├── models.py
│   ├── static
│   ├── templates
│   └── views.py
├── config.py
├── LICENSE
├── README.md
├── requirements.txt
└── run.py

3 directories, 8 files
```

