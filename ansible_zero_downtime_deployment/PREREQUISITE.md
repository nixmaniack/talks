Download and add CentOS vagrant box.

    $ wget -c  https://opscode-vm-bento.s3.amazonaws.com/vagrant/virtualbox/opscode_centos-7.0_chef-provisionerless.box
    $ vagrant box add --name centos7 opscode_centos-7.0_chef-provisionerless.box

Append hosts to `/etc/hosts`.

    172.16.3.15 web1
    172.16.3.16 web2
    172.16.3.17 db1
    172.16.3.18 lb1
    172.16.3.19 nagios


You need to have your SSH key pair located at `~/.ssh` (e.g. `~/.ssh/id_rsa.pub`)
which is used when provisioning Vagrant VMs.
