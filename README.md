macproxy
========

A simple HTTP proxy script for putting early computers on the Web. Despite its name, there is nothing Mac specific about this proxy. It was originally designed with compatibility with the MacWeb web browser in mind, but has been tested on a variety of vintage web browsers since.

The proxy.py script runs a Flask server that takes all requests and proxies them, using html_utils.py to strip tags that are incompatible with, or pulls in contents that aren't parsable by old browsers such as Netscape 4 or MacWeb.

Usage
=====
Launch the start.sh shell script to create and manage a venv Python environment, after which it will launch the proxy script.

$ ./start.sh

You may also start the Python script by itself, and use system Python.

$ python3 proxy.py
