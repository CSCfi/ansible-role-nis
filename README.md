[![Build Status](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-nis.svg?branch=master)](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-nis)
ansible-role-nis
=========

Configures NIS

Requirements
------------


Role Variables
--------------

See defaults/main.yml

Some of them:

   - nis\_enabled: True
      - If set to False don't run this role
   - nis\_initialize: True
      - initialize runs "ypinit -m servername"
   - nis\_server: True / False
      - Sets up the master, defaults to only setting up the client
   - nis\_domain: yourNISdomain

It's also possible to disable configuration of nsswitch and nscd.


Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ansible-role-nis }

License
-------

MIT

Author Information
------------------

Inspiration from:

    - https://github.com/CobraLab/ansible-playbooks
