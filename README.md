# sap-base-settings
Sets hostname &amp; locale according to SAP Note 2369910

# Variables:
- sap_hostname -- defaults to "{{ ansible_hostname }}"
- sap_domain -- defaults to "{{ ansible_domain }}"

This role checks that domainname, hostname -s and hostname -f return the correct values
This role sets the locale to en_US.UTF-8 as required in the above SAP note
