Provisioning a new site
=======================

## Required packages:

* apache (lib_proxy)
* Python 3
* Git
* pip
* virtualenv

## Apache Host Config

* See apache.http.template.conf
* Replace the site name with the appropriate name

## Upstart Job

* See gunicorn-upstart.template.conf
* Again replace site name with the appropriate name

## Gunicorn

Somewhere in here we are missing the actual installation of Gunicorn,
which is done with pip in the virtualenv.  For now gunicorn.conf is
going in the SITENAME directory (see below).  That is probably not the
right place for it.

## Folder structure:

/home/username
|--sites
   |--SITENAME
      |--database
      |--source
      |--static
      |--virtualenv
