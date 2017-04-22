Ansible Role: Percona
=====================

Ansible role to install Percona as a replacement for MySQL.

Requirements
------------

- MySQL

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    mysql_root_password: CCPQGcSV
    
Set the root password

    mysql_slow_query_log: 0
    
Turn on/off slow query log

    mysql_long_query_time: 1
    
Time in seconds before add query to slow query log

Dependencies
------------

None.

Example Playbook
----------------

    - name: Install Percona
      hosts: dbservers
      become: true
      become_method: sudo
      roles:
        - mosufy.percona

License
-------

This codebase is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)

Author Information
------------------

For any issues with installation or getting this to work, send an email to: [mosufy@gmail.com](mailto:mosufy@gmail.com)
