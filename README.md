Ansible Role: ctf-flags
=======================

Inject flags for use in CTFs. 

Requirements
------------

None

Role Variables
--------------
Available variables are listed below, along with default values (see `defaults/main.yml`):
**Required variables**:

```
flag
```
The contents of the flag, e.g `FLAG{The_flag}`

**Optional variables**:
The path of the flag
```
flag_path
```
The path to the flag. Default: `/root/flag.txt`


```
flag_owner
```
The user who owns the file. Default: `root`

```
flag_group
```
The group that owns the file. Default: `root`

```
flag_permissions
```
The permissions of the file. Default: `0400`

Dependencies
------------

None

Example Playbook
----------------
    - hosts: servers
      roles:
        - { role: ctf-flags, flag: "FLAG{THE_FLAG}" }

License
-------

BSD
