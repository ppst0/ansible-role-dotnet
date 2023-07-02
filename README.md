Ansible Role Dotnet
=========

Role to help install dotnet core

Requirements
------------

No any specific requirements for this role.

Role Variables
--------------

In *defaults/main.yml* contain following definitions:

```dotnet_package: dotnet-runtime-7.0```

Possible value for this variable is: dotnet-sdk-{Version}, dotnet-runtime-{Version}, aspnetcore-runtime-{Version}. {Version} is one of the following values: 7.0, 6.0, 5.0, 3.1.

More information about dotnet versions available for installation is here - [RHEL](https://docs.microsoft.com/en-us/dotnet/core/install/linux-package-manager-rhel7), [Debian](https://docs.microsoft.com/en-us/dotnet/core/install/linux-package-manager-debian10)

Dependencies
----------

No.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: ppst0.dotnet, dotnet_package: dotnet-sdk-3.1 }
```

License
-------

Apache 2.0

Author Information
------------------

-
