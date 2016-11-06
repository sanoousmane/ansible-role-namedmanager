Namedmanager
=========

This role installs and configures the namedmanager.
 
NamedManager is an AGPL web-based DNS management system designed to make the adding, adjusting and removal of zones/records easy and reliable.

Rather than attempting to develop a new nameserver as in the case of many DNS management interfaces, NamedManager supports the tried and tested Bind nameserver, by generating Bind compatible configuration files whenever a change needs to be applied.

This also ensures that an outage of the management server web interface or SQL database will not result in any impact to DNS servers.


More about Namedmanager
------------------------

https://github.com/jethrocarr/namedmanager


Requirements
------------

This role requires Ansible 1.9 or higher and platform requirements are listed in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows.


masternode: ns01.sanogo.net

othernode: ns02.sanogo.net 

dns: 53

http: 80

https: 443                


Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - ousmane.namedmanager-dns

License
-------

BSD

Author Information
------------------

Ousmane Sanogo http://www.sanogo.net
