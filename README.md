Role Name: sap-base-settings
=========================== =

Sets hostname and locale according to SAP Note 2369910

This is required by SAP Netweaver and SAP HANA installations

This role checks that domainname, hostname -s and hostname -f return the correct values
This role sets the locale to en_US.UTF-8 as required in the above SAP note

Requirements
------------

Prior to run this role the network and DNS settings should be done, eg. with linux-system-roles


Role Variables
--------------

- sap_hostname -- defaults to "{{ ansible_hostname }}"
- sap_domain -- defaults to "{{ ansible_domain }}"
- sap_ip -- defaults to "{{ ansible_default_ipv4.address }}"

sap_hostname is the short hostname of the SAP system and sap_domain is the DNS domainname. SAP needs both of these parameters to be checked.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: mk-ansible-roles.sap-base-settings }

License
-------

GNU GENERAL PUBLIC LICENSE
Version 3, 29 June 2007


Author Information
------------------

Markus Koch

Please leave comments in the github repo issue list
                                                                                                                                                           169,1        Ende


