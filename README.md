acme.sh
=========

Provision acme.sh script with sample template installation. Acme issue will be check on stagging server, you will have time, if you got errors.

Requements
-------------

- debian-based system
- Set-uped hostname on target server.

Role Variables
--------------

If varable is defined - trigger will work. Group vars must working.

Inventory
------------

	[es]
	es.33slona.ru rewrite_ssl=True rewrite_www=True

Example Playbook
----------------

	- hosts: servers
	  roles:
	     - egeneralov.acme


License
-------

MIT

Author Information
------------------

Eduard Generalov <eduard@generalov.net>
