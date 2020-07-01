=============
ROLE GRAPHITE
=============

.. image:: https://img.shields.io/github/license/adfinis-sygroup/ansible-role-graphite.svg?style=flat-square
  :target: https://github.com/adfinis-sygroup/ansible-role-graphite/blob/master/LICENSE

.. image:: https://img.shields.io/travis/adfinis-sygroup/ansible-role-graphite.svg?style=flat-square
  :target: https://github.com/adfinis-sygroup/ansible-role-graphite

.. image:: https://img.shields.io/badge/galaxy-adfinis--sygroup.graphite-660198.svg?style=flat-square
  :target: https://galaxy.ansible.com/adfinis-sygroup/graphite

Installs and configures a basic setup with carbon, graphite-web and whisper.


Requirements
=============

This role has no requirements.

Role Variables
===============

.. code-block:: ini

  graphite_web_db_name: "/opt/graphite/storage/sqlite.db"
  graphite_web_db_user: "graphite"
  graphite_web_db_password: "passw0rd"
  graphite_web_db_host: "localhost"
  graphite_web_db_port: ""
  graphite_web_db_engine: "django.db.backends.sqlite3"
  graphite_web_db_ssl: False
  graphite_web_db_ssl_ca: "/etc/ssl/certs/ca-bundle.crt"
  graphite_web_timezone: "Europe/Zurich"
  graphite_web_salt: "&lt;random salt&gt;"

Dependencies
=============

This role has no direct dependency to other roles.

Example Playbook
=================

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

.. code-block:: yaml

  - hosts: servers
    roles:
       - { role: adfinis-sygroup.graphite }


License
========

`GPL-3.0 <https://github.com/adfinis-sygroup/ansible-role-graphite/blob/master/LICENSE>`_


Author Information
===================

graphite role was written by:

* Adfinis AG | `Website <https://www.adfinis.com/>`_ | `Twitter <https://twitter.com/adfinis>`_ | `GitHub <https://github.com/adfinis-sygroup>`_

