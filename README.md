Geo citizen web
=========
Ansible role for configuring Ubuntu 20.04 with Java, Tomcat, Maven for project **Geo citizen**

Requirements
------------

Tested in AWS EC2, other environment does not guarantee proper working, but you can test.
Role Variables
--------------

This role requires following variables:
```
email_login: YOUR_EMAIL@LOGIN
email_password: YOUR_EMAIL_PASSWORD
db_user: DATABASE_USERNAME
db_password: DATABASE_USER_PASSWORD
db_name: DATABASE_NAME
```

Dependencies
------------

Geo citizen db ansible role should be used to configure full project
Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- name: WEB
  hosts: web
  become: true
  vars_files: secret_vars.yml
  roles:
    - geo_web
```

License
-------

MIT

Author Information
------------------
Vladyslav Karpenko
