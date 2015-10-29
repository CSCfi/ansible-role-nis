ansible-role-nis
=========

Configures NIS

Requirements
------------


Role Variables
--------------

   - nis\_enabled: True
      - If set to False don't run this role
   - nis\_initialize: True
      - initialize runs "ypinit -m servername"
   - nis\_server: True / False
      - Sets up the master, defaults to only setting up the client
   - nis\_domain: yourNISdomain


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
