===========
Newebe
===========
:Info: Newebe is a (almost) distributed social platform.
:Author: Gelnior (http://gelnior.wordpress.com)
:License: AGPL v3.0


Dependencies
============
* python >= 2.6
* django >= 1.2
* couchdb >= 0.11.0
* coucdbkit >= 0.4.8


Set up a development environment (Ubuntu 10.4)
==============================================
Install following packages:

    python python-django python-couchdbkit couchdb git

You can also install *couchbkit* via *easy_install*:

    easy_install -U Couchdbkit

Create a Couchdb database called *newebe* (case sensitve) via *Futon*
(http://localhost:5984/_utils).

Retrieve Newebe project:

   git clone http://github.com/gelnior/newebe.git 

In Newebe directory run:

   python manage.py syncdb

Then, still in Newebe directory run:

   python manage.py runserver

Run tests suite: 

   python manage.py test platform news

In your browser, connect to http://localhost:8000/ and check that 
everything is fine.

