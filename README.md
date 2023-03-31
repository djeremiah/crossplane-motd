ansible-role-crossplane-motd
=========

This role adds a [Crossplane](https://crossplane.io) banner to the message of the day on Linux systems.

Requirements
------------

None

Role Variables
--------------

Available variables are listed below, with default values (see [defaults/main.yml](defaults/main.yml))

The destination directory where motd fragments are stored

    destination: /etc/update-motd.d

The lexical priority for the banner. This value will be used to construct the final filename using a template `${destination}/${priority}-crossplane`, i.e. `/etc/update-motd.d/99-crossplane`

    priority: 99


Dependencies
------------

None

License
-------

MIT-0
