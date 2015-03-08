jpic.pacmanrepo
===============

Signed package repository for Arch Linux used for
Yourlabs package repository.

Requirements
------------

- pacmanrepo_name: A repository name of your choice.
  This is what users will have to add in pacman.conf
  between brackets, ie. `[yourlabs]`.

Role Variables
--------------

- pacmanrepo_source: local path to search for signed
  packages.
- pacmanrepo_destination: remote path where your repo
  is hosted.
- pacmanrepo_architectures: defaults to i686, x86_64, any.

Dependencies
------------

`jpic.pacman` and `jpic.gpg` are optionnal but I don't see why you'd use one
without the other.

Example Playbook
----------------

Example using the corresponding `jpic.pacman` role configuration:

.. include:: Vagrantplaybook.yml

License
-------

BSD
