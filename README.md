Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

| Variable                              | Default                       | Notes				|
| :---                                  | :---                          | :---				|
| varnish_listen_address		| ''				| '' binds to all		|
| varnish_listen_port			| 6081				|    	      			|
| varnish_admin_listen_address		| 127.0.0.1			|				|
| varnish_admin_listen_port		| 6082				|				|
| varnish_backend_host			| 127.0.0.1			|				|
| varnish_backend_port			| 80				|				|

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)
