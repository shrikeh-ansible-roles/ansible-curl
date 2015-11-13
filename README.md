# ansible-curl
[![Galaxy](http://img.shields.io/badge/galaxy-shrikeh.curl-blue.svg)] [galaxy]
[![Build Status](https://img.shields.io/travis/shrikeh/ansible-curl.svg)][build_status]
[![GitHub Stars](https://img.shields.io/github/stars/shrikeh/ansible-curl.svg)][github]

Installs cURL on hosts in a cross-playform way.

## Requirements
------------

None.

## Role Variables
--------------

#### [`curl_pkg_state_latest`][curl_pkg_state_latest]
Default: `no`
Controls whether to use 'present' or 'latest' for package installation.

#### [`curl_update_pkg_mgr`][curl_update_pkg_mgr]
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
 -------

 [MIT][licence]

Author Information
------------------
Feel free to hit me up on Twitter @barney_hanlon

[galaxy]: https://galaxy.ansible.com/list#/roles/4384 "Ansible Galaxy"
[build_status]: https://travis-ci.org/shrikeh/ansible-curl "Build status on travis"
[github]: https://github.com/shrikeh/ansible-curl "cURL role on Github"
[curl_pkg_state_latest]: https://github.com/shrikeh/ansible-curl/blob/master/defaults/main.yml#L2 "Variable definition in defaults.yml"
[curl_update_pkg_mgr]: https://github.com/shrikeh/ansible-curl/blob/master/defaults/main.yml#L3 "Variable definition in defaults.yml"
