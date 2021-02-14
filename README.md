ansible-role-sway
=========

This role installs and configures the sway tiling window manager and it's dependencies. For some programs, it is also possible to compile them from source.

Requirements
------------

It is required to run one of the supported distros and have a config file for sway (or other programs that you are looking to use)

Role variables
--------------

Please consult vars/<distribution-name> for variable options

Config files must be placed in the files folder in folders, like this:

files
├── mako
│   └── config
├── sway
│   ├── config
│   └── themes
│       └── gruvbox

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      roles:
         - role: ansible-role-sway

License
-------

MIT
