Django CMS site
===============

Django CMS site suitable for Docker

`www.django-cms.cz <https://www.django-cms.cz/>`__

`Docker image <https://hub.docker.com/r/misli/django-cms-site/>`__


Installation with pip
---------------------

.. code:: shell

    # create and enter an empty directory of your choice
    mkdir django-cms && cd django-cms

    # create and activate virtual environment
    virtualenv env
    . env/bin/activate

    # install django-cms-site with all the requirements
    pip install django-cms-site

    # create database
    django-cms migrate

    # create admin user
    django-cms createsuperuser

    # run development server
    DEBUG=TEMPLATE django-cms runserver
