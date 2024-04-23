Role Name
=========

Easy install any binary from release archive.


Why ?
---

Because package manager may not have your app or expected version.


Example Playbook
----------------


```yml
  - hosts: servers
    roles:
    - role: sohelzerdoumi.release_installer
      archive_url: https://github.com/neovim/neovim/releases/download/v0.9.5/nvim-linux64.tar.gz
      binary_filename: bin/nvim
```

Requirements
------------

None.

Role Variables
--------------

| Variable                  | Description                       |
|---------------------------|-----------------------------------|
| `archive_url`             | Url to download                   |
| `archive_binary_filepath` | Filename of binary inside archive |
| `install_path`            | Target path to installed binary   |


Dependencies
------------

None.

Todo
-----

[ ] Provide extra files to install (ex: lib/ man/ etc...)


License
-------

MIT
