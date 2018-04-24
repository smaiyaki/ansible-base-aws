ansible-base-aws
================

This role aims to do basic tasks on any host running on AWS. This includes
installing basic dependencies and/or extra pip/packages on the system; and
setting up the host file, hostname, r53 entries.

Role Variables
--------------

**base_deps**

When set to true it will try installing extra packagesd defined afterwards
default: ``true``

**base_extra_packages**

The extra packages (deb/rpm) to install

default: ``[]``

**base_extra_pip_packages**

The extra pip packages to install

default: ``[]``

**base_hosts**

If host settings should be included

default: ``false``

**base_hosts_suffix**

Specify if you want specific hosts suffix

default: ``""``

**base_manage_host_file**

Set to true if you want the hosts file to be managed

default: ``true``

**base_manage_host_r53**

Set to true if you want internal entries to be created

default: ``false``

**base_r53_internal_zone**

Defines in which internal zone entries should be added in R53

default: ``""``

**base_custom_hosts**

Define extra custom hosts for the /etc/hosts file to fill with
default: ``{}``

License
-------

MIT

Author Information
------------------

Hugo Rosnet at Cycloid.io
