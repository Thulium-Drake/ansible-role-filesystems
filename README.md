## Filesystems in LVM, powered by Ansible
This role provides a means to configure filesytems in LVM Logical Volumes.

This role will take care of the following:

  - Creating/expanding Volume Groups with Physical Volumes (NOTE: _not_ creating/expanding Physical Volumes themselves)
  - Creating/expanding Logical Volumes
  - Creating a mountpoint
  - Formatting a filesystem (NOTE: only on _new_ Logical Volumes)
  - Ensuring the Logical Volume is mounted

DISCLAIMER: It's not my fault if this role eats your homework or kills your dog!

The main purpose of this role is to manage (mostly extend) existing LVMs on a system to have their sizes managed centrally. It can also be used to create new filesystems if need be, however, be cautious and don't run this without testing what happens with your existing storage!

See defaults/main.yml for more information on what to configure where and how.
