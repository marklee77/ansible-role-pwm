marklee77.pwm
=============

The purpose of this role is to install pwm to a web server and enable
access with nginx. This install uses the MySQL backend. The pwm server name
can be specified by changing the pwm_hostname variable in
defaults/main.yml.

This role is still in development and is not currently functional.

Role Variables
--------------

- pwm_hostname: hostname that pwm will service, will be set to 
                       "pwm" by default
- pwm_port: hostname that pwm will service, will be set to 8888 by 
               default.
- pwm_root_mysql_password: root mysql password, will be set to a random 
                                value by default.
- pwm_pwm_mysql_password: pwm mysql password, will be set to a 
                                    random value by default.
* pwm_admin_login: pwm admin login name, 'root' by default.
- pwm_admin_password: pwm admin password, 'password' by default.

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables 
passed in as parameters) is always nice for users too:

    - hosts: default
      sudo: True
      roles:
        - pwm

Try it Out
----------

Check out the github repository, vagrant up, and load http://localhost:8888 in
your web browser.

License
-------

GPLv2

Author Information
------------------

http://stillwell.me

