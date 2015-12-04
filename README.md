# ansible-curl
[![Galaxy](http://img.shields.io/badge/galaxy-shrikeh.curl-blue.svg)] [galaxy]
[![Build Status](https://img.shields.io/travis/shrikeh-ansible-roles/ansible-curl.svg)][build_status]
[![GitHub Stars](https://img.shields.io/github/stars/shrikeh-ansible-roles/ansible-curl.svg)][github]

Low-level [Ansible][ansible] role to install [cURL][curl] on hosts in a cross-platform way.

## Requirements
------------

None.

## Role Variables
--------------

##### [`curl_pkg_state_latest`][curl_pkg_state_latest]
Default: `no`
Controls whether to use 'present' or 'latest' for package installation.

##### [`curl_update_pkg_mgr`][curl_update_pkg_mgr]
Default: `no`
Whether or not to update package managers prior to running this.

## Dependencies
------------

None.

## Example Playbook
----------------
```YAML
    - hosts: servers
      vars:
        curl_pkg_state_latest: yes
      roles:
         - { role: shrikeh.curl }
```

## License

[MIT][licence]

## Author Information

Contact me on Twitter @[barney_hanlon][twitter]

[ansible]:http://www.ansible.com/ "Ansible home page"
[galaxy]: https://galaxy.ansible.com/list#/roles/4384 "Ansible Galaxy"
[curl]: http://curl.haxx.se/ "cURL home page"
[licence]: https://raw.githubusercontent.com/shrikeh/ansible-curl/master/LICENSE "Link to the license in the repository"
[build_status]: https://travis-ci.org/shrikeh-ansible-roles/ansible-curl "Build status on travis"
[github]: https://github.com/shrikeh-ansible-roles/ansible-curl "cURL role on Github"
[curl_pkg_state_latest]: https://github.com/shrikeh-ansible-roles/ansible-curl/blob/master/defaults/main.yml#L2 "Variable definition in defaults.yml"
[curl_update_pkg_mgr]: https://github.com/shrikeh-ansible-roles/ansible-curl/blob/master/defaults/main.yml#L3 "Variable definition in defaults.yml"
