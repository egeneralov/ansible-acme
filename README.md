acme.sh
=========

Provision acme.sh script with sample template installation.

acme.sh will be check on stagging server, you`l have time, if you got errors.

For now working only on debian-based, tested on debian {8,9}

Requements
-------------

Normal FQND on target.

Installation
-------------

	ansible-galaxy install -f git+ssh://git@git.33slona.ru:49384/ansible/ansible-roles/acme.sh.git

Role Variables
--------------

If varable is defined - trigger will work. Group vars must working.

Inventory
------------

	[es]
	es.33slona.ru rewrite_ssl=True rewrite_www=True

Example Playbook
----------------

	---
	- hosts: es
	  roles:
	     - acme.sh


License
-------

MIT

Author Information
------------------

Eduard Generalov
