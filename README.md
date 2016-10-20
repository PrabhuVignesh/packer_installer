packer_installer
=========

Packer is an open source tool for creating identical machine images for multiple platforms from a single source configuration.
	
Packer is lightweight, runs on every major operating system, and is highly performant, creating machine images for multiple platforms in parallel. Packer does not replace configuration management like Chef or Puppet. In fact, when building images, Packer is able to use tools like Chef or Puppet to install software onto the image.


Requirements
------------
1. Ansible need to be installed
2. Clester of nodes and it's hostname shoud get entry into your inventory file

Role Variables
--------------

default variables: (can be changed while running playbook)

1. unzip_version: "6.0*"
2. packer_binary_link: "https://releases.hashicorp.com/packer/0.10.2/packer_0.10.2_linux_amd64.zip"

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: prabhuvignesh.packer_installer, x: 42 }

License
-------

Opensource

Author Information
------------------

..*Prabhu Vignesh Kumar Rajagopal
..*http://prabhuvignesh.github.io
