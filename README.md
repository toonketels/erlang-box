Vagrant Ubuntu erlang
===========================

Sets up an ubuntu with erlang for development purposes.

Needs to have the following roles installed:

    ansible-galaxy install stwind.erlang

To run do:

    vagrant up

To reprovision do:

    vagrant provision

To issue ad-hoc commands via ansible do:

    ansible -i .vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory -u vagrant --private-key=~/.vagrant.d/insecure_private_key default -a 'ls'
