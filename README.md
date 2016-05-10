# ansible-nginx-passenger
=======================

This role does the following:

- Install `nginx`
- Install `passenger`
- Enable `passenger` config
- Install `nginx init.d service`

Supportes SOs
-------------
Tested on `ubuntu/trusty64` but migth work as well in othes debian based distros

Role Variables
--------------
None.

Dependencies
------------
You need a `ruby` installation before the `passenger` setup.

Usage
-----
Include this role in a playbook as below:

    - hosts: servers
      roles:
         - { role: spireworks.nginx-passenger, become: yes }

Testing
-------
You need to install `vagrant` in your local machine. Just run
`vagrant up` and go and get a coffee. If you want go provision an
existing machine, run `vagrant provision`. Remember to
run `vagrant destroy` so you don't run out of RAM in your
laptop ;)

License
-------
MIT
