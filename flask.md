---
title: "Flask"
---

# Get started

Clone this project:

```sh
$ git config --global http.sslVerify "false" # only at school!
$ git clone https://github.com/lamerce/webapp-python.git
```

If you don't have sudo rights, then add `~/.local/bin` to your `$PATH` (if needed) and install 

```sh
$ echo 'export PATH="$HOME/.local/bin:$PATH"' >> $HOME/.bashrc
$ source $HOME/.bashrc
$ cd webapp-python
$ pip install --user -r requirements-dev.txt
```

If you have sudo rights, use a virtual environment:

```sh
$ sudo apt install python3-venv
$ cd webapp-python
$ python3 -m venv .venv
$ source .venv/bin/activate
(.venv) $ python3 -m pip install --upgrade pip
(.venv) $ pip install -r requirements-dev.txt
```

Start the web app:

```sh
$ flask run
* Environment: production
  ...
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```

Fire up a web browser and navigate to [http://localhost:5000](http://localhost:5000)

# Documentation

[Flask](https://flask.palletsprojects.com/en/2.0.x/quickstart/). Flask is a micro web framework written in Python.

[Templates](https://jinja.palletsprojects.com/en/3.0.x/templates/). Jinja is a fast, expressive, extensible templating engine. Special placeholders in the template allow writing code similar to Python syntax. Then the template is passed data to render the final document.