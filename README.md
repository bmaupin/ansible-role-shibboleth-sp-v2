Ansible role for Shibboleth SP

### Features

- Installs the latest version of Shibboleth SP (currently v3)
- Installs httpd and PHP
- Installs minimal attribute viewer from https://github.com/bmaupin/shibboleth-attribute-viewer


### Requirements

- CentOS 7


### Instructions

1. Include the role and customize templates/shibboleth2.xml.j2 as desired

2. Configure SP with an IdP. You can get the medatadata from here:
    - http://hostname/Shibboleth.sso/Metadata (Replace hostname with the hostname of your SP)

3. Browse to http://hostname/secure/ to test Shibboleth login and view attributes


### Sample playbook

    - hosts: shibboleth-sp-servers
      roles:
        - shibboleth-sp
