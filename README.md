troykinsella.docker-machine
===========================

An ansible role to install docker-machine by binary download.

Role Variables
--------------

* docker_machine_version: The docker-machine version to install. Default: 0.6.0.
* docker_machine_os: The OS for which to select the binary. Default: linux.
* docker_machine_architecture: The architecture for which to select the binary. Default: x86_64.
* docker_machine_url: The URL at which the binary can be downloaded. Default: the official source according to OS and architecture variables.
* docker_machine_binary_path: The full path to the installed docker-machine binary. Default: /usr/local/bin/docker-machine.
* docker_machine_binary_mode: The file mode of the docker-machine binary. Default: 0755.
* docker_machine_binary_user: The docker-machine binary user. Default: root.
* docker_machine_binary_group: The docker-machine binary group: Default: root.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: troykinsella.docker-machine
           docker_machine_version: 0.6.0

License
-------

MIT
