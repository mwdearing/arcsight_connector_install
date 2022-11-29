CONNECTOR_INSTALL
=========

This role deploys a silent.properties file for a silent install of the ArcSight Connector Framework. 

Requirements
------------

| Name        | Default Values                                | Description           |
| ----------- | --------------------------------------------- | --------------------- |
| connector   | "test_1"                                      | Base connector folder |
| install_dir | "/opt/arcsight/connectors/"                   | Full install URI      |
| binary      | "ArcSight-8.4.0.8955.0-Connector-Linux64.bin" | Binary Name           |
| remote_port | "9005"                                        | Remote port           |

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

None

Example Playbook
----------------


    - hosts: all
      vars:
        - connector: "connector_1"
        - install_dir: "/opt/arcsight/connectors/"
        - binary: "ArcSight-8.4.0.8955.0-Connector-Linux64.bin"
        - remote_port: "9001"
      roles:
         - role: roles/connector_install

License
-------

MIT