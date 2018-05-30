Ansible role for Shibboleth SP

### Features

- Installs Shibboleth SP
- Installs httpd and PHP
- Installs minimal attribute viewer from https://github.com/bmaupin/shibboleth-attribute-viewer


### Instructions

1. Include the role and customize files/shibboleth2.xml as desired

2. Browse to http://hostname/secure/ to test Shibboleth login and view attributes


### Sample playbook

    - hosts: shibboleth-sp-servers
      roles:
        - shibboleth-sp
