# install-debs
This role copies and installs some loose deb packages.

## Requirements
The target host needs to be running Debian or a derived system (in particular,
it needs to support the `apt` task).

## Role Variables

### Required Variables
* `install_debs` *list of strings* - list of deb files on the local system

### Optional Variables
* `install_debs_cache_dir` *string* - path on the target system where the debs
  are stored, defaults to `~/.cache/install-debs`

## Example
    - role: install-debs
      install_debs:
        - debs/a.deb
        - debs/b.deb

## License
This software is licensed under the 2-clause BSD license. See the accompanying
`LICENSE.md` file.
Copyright (c) 2017, Felix Krull. All rights reserved.
