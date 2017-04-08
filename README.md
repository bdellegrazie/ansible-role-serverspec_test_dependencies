# serverspec_test_dependencies [![Build Status](https://travis-ci.org/bdellegrazie/ansible-role-serverspec_test_dependencies.svg?branch=master)](https://travis-ci.org/bdellegrazie/ansible-role-serverspec_test_dependencies)

Install dependencies needed to execute [ServerSpec](http://serverspec.org/) tests on a target.
Note this _does not_ install Ruby or ServerSpec. This only installs dependencies needed for the tests themselves
It is useful for situations such as executing tests on docker containers where the serverspec binaries are
installed on the host and the tests are being executed via the docker cli

## Dependencies

None

## Example Playbook

Usually this will be part of the test suite definition:

    - hosts: servers
      roles:
         - { role: serverspec_test_dependencies }

## License

GPLv3

## Author

[Brett Delle Grazie](https://github.com/bdellegrazie/ansible-role-serverspec_test_dependencies)
