# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    # Debian 9 Server
  config.vm.define "debian9" do |config|
    config.vm.box = "geerlingguy/debian9"

    config.ssh.insert_key = false

    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    config.vm.hostname = "geerlingguy-debian9.test"
    config.vm.network :private_network, ip: "192.168.60.10"
  end

  # Debian 10 Server
  config.vm.define "debian10" do |config|
    config.vm.box = "geerlingguy/debian10"

    config.ssh.insert_key = false

    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    config.vm.hostname = "geerlingguy-debian10.test"
    config.vm.network :private_network, ip: "192.168.60.11"
  end

  # CentOS 7 Server
  config.vm.define "centos7" do |config|
    config.vm.box = "geerlingguy/centos7"

    config.ssh.insert_key = false

    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    config.vm.hostname = "geerlingguy-centos7.test"
    config.vm.network :private_network, ip: "192.168.60.21"
  end

  # CentOS 8 Server
  config.vm.define "centos8" do |config|
    config.vm.box = "geerlingguy/centos8"

    config.ssh.insert_key = false

    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    config.vm.hostname = "geerlingguy-centos8.test"
    config.vm.network :private_network, ip: "192.168.60.22"
  end
end
