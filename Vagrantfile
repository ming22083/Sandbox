# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-7.1"

  config.vm.box_check_update = false

  config.vm.provider :virtualbox do |vb|
    vb.customize ["modifyvm", :id, "--vram", 16]
    vb.customize ["modifyvm", :id, "--memory", "2048"]
    vb.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
    vb.gui = false
  end

  config.vm.network "forwarded_port", guest: 80, host: 80
  config.vm.network :private_network, ip: "192.168.33.220"
  config.vm.hostname = "ming.dev"
  config.hostsupdater.aliases = [
    "ming.dev"
  ]
end
