PHP
========

Install latest PHP version in DotDeb repository

Requirements
------------

Debian Wheezy with the package python-pycurl and python-software-properties installed.

Role Variables
--------------

There are as many role variables as PHP.ini variables. All of them can be set, but the defaults
are adjusted according to [iniscan](https://github.com/psecio/iniscan) security best practices.

Dependencies
------------

Depends on f500.repo_dotdeb.

Example Playbook
-------------------------

    - hosts: servers
      roles:
         - { role: f500.php, php_error_reporting: "E_ALL" }

License
-------

LGPL

Author Information
------------------

Jasper N. Brouwer, jasper@nerdsweide.nl

Ramon de la Fuente, ramon@delafuente.nl
