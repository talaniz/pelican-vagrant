Pelican Vagrant
==================

A role to setup a Pelican blog on Vagrant or a live server.

Requirements
------------

Ansible version 16+ as the ufw module is used.

Variables
---------

* `pelican_env`: directory where virtualenv is installed
* `pelican_themes`: location of pelican themes to be installed
* `web_root`: root folder for the web server
* `blog_repo`: repo to clone to create the pelican blog

Example Playbook
----------------

    - hosts: servers
      vars:
         - pelican_env: /home/user1/pelican/bin/python
         - pelican_themes: /home/themes
         - web_root: /var/www/mysite/output
         - blog_repo: https://github.com/talaniz/ansible-pelican.git
      roles:
         - talaniz.pelican-vagrant

License
-------

BSD

Author Information
------------------
E-mail: antonio.alaniz@gmail.com
Website: www.antonioalaniz.com

