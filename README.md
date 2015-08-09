correcthorse.varnish
=========

A role for installing varnish cache. It doesn't do anything fancy with VCL, it is expected that you will use varnish_vcl_includes to include some custom vcl files that you manage in your master playbook.

Role Variables
--------------

| Variable                              | Default                       | Notes				|
| :---                                  | :---                          | :---				|
| varnish_upstream_repo			| false				| use false (epel) for centos 7	|
| varnish_listen_address		| ''				| '' binds to all		|
| varnish_listen_port			| 6081				|    	      			|
| varnish_open_port			| false				|				|
| varnish_admin_listen_address		| 127.0.0.1			|				|
| varnish_admin_listen_port		| 6082				|				|
| varnish_backend_host			| 127.0.0.1			|				|
| varnish_backend_port			| 80				|				|
| varnish_vcl_includes			| []				| List of vcl files to include, dummy files are created when they don't exist to makes sure varnish can start |

Dependencies
------------

- correcthorse.common

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: correcthorse.varnish }

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)
