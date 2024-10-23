## Filesystems in LVM, powered by Ansible
This role provides a means to configure filesytems in LVM Logical Volumes.

This role will take care of the following:

  - Creating/expanding Volume Groups with Physical Volumes (NOTE: _not_ creating Physical Volumes themselves)
  - Creating/expanding Logical Volumes
  - Creating a mountpoint
  - Formatting a filesystem (NOTE: only on _new_ Logical Volumes)
  - Ensuring the Logical Volume is mounted
