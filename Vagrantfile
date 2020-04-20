# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # Debian 10 Server
  config.vm.define "debian10" do |debian10|
    debian10.vm.box = "geerlingguy/debian10"

    debian10.ssh.insert_key = false
  
    debian10.vm.synced_folder ".", "/vagrant", disabled: true
  
    debian10.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    debian10.vm.hostname = "debian10.test"
    debian10.vm.network :private_network, ip: "192.168.60.10"
  end

  # CentOS 7 Server
  config.vm.define "centos7" do |centos7|
    centos7.vm.box = "geerlingguy/centos7"

    centos7.ssh.insert_key = false
  
    centos7.vm.synced_folder ".", "/vagrant", disabled: true
  
    centos7.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    centos7.vm.hostname = "centos7.test"
    centos7.vm.network :private_network, ip: "192.168.60.11"
  end
  
  # CentOS 8 Server
  config.vm.define "centos8" do |centos8|
    centos8.vm.box = "geerlingguy/centos8"

    centos8.ssh.insert_key = false
  
    centos8.vm.synced_folder ".", "/vagrant", disabled: true
  
    centos8.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    centos8.vm.hostname = "centos8.test"
    centos8.vm.network :private_network, ip: "192.168.60.12"
  end
end