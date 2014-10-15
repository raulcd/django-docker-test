Django Docker Test
==================

Django docket test is a test to build a django application with docker.

It uses docker to build the containers and fig to orchestrate.

Requirements
============

* First, you need docker installed. See http://docs.docker.com/installation/ubuntulinux/
* Second, you need fig installed. See http://www.fig.sh/install.html.

Usage
=====

Turn on your containers:

```
fig up
```

To run the containers in detached mode:

```
fig up -d
```

To synchronize your database once the containers are running:

```
fig run web python manage.py syncdb
```
