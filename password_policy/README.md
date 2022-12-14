Role Name
=========

Ansible role to setup password policy in linux

Requirements
------------

Should work with most platforms ( Tested in Debian/Ubuntu and Centos )

Role Variables
--------------
Edit 
  defaults/main.yml

```bash
---
# defaults file for password_policy
password_expiration_file: /etc/login.defs
password_history_file: ''
password_complexity_file: ''

# password complexity
minlen: 8
lcredit: -1
ucredit: -1
dcredit: -1
ocredit: -1

# password history
remember: 5

# password expiration
PASS_MAX_DAYS: 60
PASS_MIN_DAYS: 0
PASS_MIN_LEN: 8
PASS_WARN_AGE: 7

```

Dependencies
------------

ToCheck and upate

Example Setup
----------------


    - hosts: servers
      roles:
         - password_policy

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
