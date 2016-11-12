# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"
VAGRANT_BOX = "centos/6"
VAGRANT_BOX_URL=""

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = VAGRANT_BOX
  #config.vm.box_url = VAGRANT_BOX_URL
 
  config.vm.define :centos do |node|
    node.vm.network :forwarded_port, guest: 22, host: 2001, id: "ssh"
    node.vm.network :private_network, ip: "192.168.33.11"
  end
end
