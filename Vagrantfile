# -*- mode: ruby -*-
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-20.04"
  #config.vm.box = "segment-routing/ubuntu-16.04"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "4024"
  end

  config.vm.synced_folder "./scripts", "/root/scripts"
  config.vm.provision "shell", privileged: true, path: "./setup.sh"
end
