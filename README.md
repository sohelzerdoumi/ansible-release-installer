Role Name
=========

Easy install any binary from release archive.


Why ?
---

Because package manager may not have your app or expected version.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

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

| Variable              | Description                       |
|-------------------------------------|-----------------------------------------------------------------|
| `archive_url`          | Url to download |
| `binary_filename` | Filename of binary inside archive |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.


Todo
-----

[ ] Provide extra files to install (ex: lib/ man/ etc...)


License
-------

MIT
