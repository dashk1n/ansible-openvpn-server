openvpn server
=========

Installing openvpn server on Ubuntu. Generate clients keys and OVPN files.
Send files to clients by email if needed.

Role Variables
--------------

See 'defaults/main.yml'
Custom variables are stored in the 'openvpn-vars.yml'

Examples
----------------
To run playbooks you have to prepare openvpn-vars.yml config file.
See openvpn-vars.yml.example

To install openvpn server and init PKI:

**ansible-playbook -i openvpn-server/hosts openvpn-server/openvpn-server.yml**

Generate vpn clients and send ovpn configs.
User's list can be defined in the file 'openvpn-vars.yml'

**ansible-playbook -i openvpn-server/hosts openvpn-server/openvpn-clients.yml**