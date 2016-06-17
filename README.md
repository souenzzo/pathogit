Pathogit
=========

Install pathogen and plugins.

Requirements
------------

Ansible and `git_module` working

Role Variables
--------------

vim dir: "{{ ansible_env.HOME }}/.vim"

vimrc: "{{ ansible_env.HOME }}/.vimrc"

plugins dir: "{{ ansible_env.HOME }}/.vim/bundle"


Dependencies
------------

nil

Example Playbook
----------------
``` yml
    - hosts: workplace
      roles:
         - role: souenzzo.pathogit
           pathogen_plugins:
             - repo: "https://github.com/Shougo/neocomplete.vim.git"
               name: custom_name ## default: neocomplete.vim
               version: custom_tag ## default: master
```

License
-------

GPLv3

Author Information
------------------

Contact, bug: https://github.com/souenzzo/pathogit
