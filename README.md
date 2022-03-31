galaxy-telegraf - stealed from https://stdio.space/ansible-galaxy/galaxy-telegraf/src/commit/41e4f237ccb55bc09542a70352c1e5be8ff93de5
===============

Install Telegraf on Debian

Requirements
------------

An InfluxDB service up and running

Role Variables
--------------

- db_name: influx db name
- db_user: influx db username
- db_pass: influx db password
- influx_host: influx host
- influx_port: influx db port
- influx_host: influx db host

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: galaxy-telegraf

Run tests
---------

Needs galaxy-vagrant to run tests

Ensure galaxy-vagrant is up

    ansible-playbook -i tests/inventory tests/test.yml
