gunicorn
=========

This role will download and install gunicorn for you, and gives you a few
options for configuring a gunicorn service.

Requirements
------------

None.

Role Variables
--------------

See the values provided in [defaults/main](defaults/main.yml). Each value should
have comments describing their use. One big exception to this is the values that
will be placed in the gunicorn config files. These values are the same as the
gunicorn values, but with names prefixed with `gunicorn_`. If you would like to
know more about those options, it would be best to go dig into the [gunicorn
documentation](https://docs.gunicorn.org/en/stable/configure.html) rather that
look here.

Dependencies
------------

None.

Example Playbook
----------------

Eg.

    - hosts: servers
      roles:
         - { role: dudefellah.gunicorn, gunicorn_service_name: my-web-service }

    ... etc etc

License
-------

GPLv2+

Author Information
------------------

Dan - github.com/dudefellah
