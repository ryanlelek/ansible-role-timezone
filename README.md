Timezone
========

Configures Timezone

IMPORTANT!
----------
**Using ANY value besides the default (Etc/UTC) is NOT RECOMMENDED.**  
Leave it as the default unless you have a specific reason to change it.  
WHATEVER you do, at least **be consistent** with the timezone you choose (Etc/UTC HIGHLY recommended).  
See [Setting the Timezone](http://www.ansibletutorials.com/setting-the-timezone/) for more information.

Requirements
------------

None

Role Variables
--------------

**timezone_locale**: Etc/UTC

Dependencies
------------

None

Example Playbook
----------------

**Default, Recommended!**

    - hosts: all
      roles:
         - ryanlelek.timezone

Not recommended, but if you want to change locales:

    - hosts: all
      roles:
         - role: ryanlelek.timezone
           timezone_locale: America/Los_Angeles

License
-------

MIT

Author Information
------------------

Created by [Ryan Lelek](https://www.ryanlelek.com)  
Part of [AnsibleTutorials.com](http://www.ansibletutorials.com)
