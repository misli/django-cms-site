Django CMS site
===============

Django CMS site suitable for Docker

[www.django-cms.cz](https://www.django-cms.cz/)


Installation with docker-compose
--------------------------------

```shell
# create and enter an empty directory of your choice
mkdir django-cms && cd django-cms

# download docker-compose configuration
wget https://raw.githubusercontent.com/misli/django-cms-site/master/docker-compose.yml

# configure the passwords
vim docker-compose.yml

# start the application containers
# (you need docker-compose installed and docker service running)
sudo docker-compose up -d

# create superuser account
sudo docker-compose exec cms django-cms createsuperuser

# once the initial migration is finished (may take few minutes),
# you should be able to open http://127.0.0.1:8000/ in your favorite browser.

# when finished stop the appliaction containers
sudo docker compose down
```
