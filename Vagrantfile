# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "xubuntu-16.04-desktop-amd64"
  config.vm.box_url = "https://github.com/akzero53/xubuntu-16.04-vagrant-box/releases/download/v1.0.0/xubuntu-16.04-desktop-amd64.box"

  config.omnibus.chef_version=:latest
  config.vm.provision "chef_solo" do |chef|
    chef.roles_path = ["roles"]
    chef.add_role("java")
    chef.add_role("idea")
    chef.add_role("git")
  end

  config.vm.provider "virtualbox" do |vb|
    vb.gui = true
    vb.memory = "2048"
  end
end
