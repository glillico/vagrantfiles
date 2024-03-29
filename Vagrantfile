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

  # Debian 11 Server
  config.vm.define "debian11" do |config|
    config.vm.box = "geerlingguy/debian11"

    config.ssh.insert_key = false

    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    config.vm.hostname = "geerlingguy-debian11.test"
    config.vm.network :private_network, ip: "192.168.60.12"
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
    config.vm.network :private_network, ip: "192.168.60.20"
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
    config.vm.network :private_network, ip: "192.168.60.21"
  end

  # Ubuntu 18.04 Server
  config.vm.define "ubuntu1804" do |config|
    config.vm.box = "geerlingguy/ubuntu1804"

    config.ssh.insert_key = false

    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    config.vm.hostname = "geerlingguy-ubuntu1804.test"
    config.vm.network :private_network, ip: "192.168.60.30"
  end

  # Ubuntu 20.04 Server
  config.vm.define "ubuntu2004" do |config|
    config.vm.box = "geerlingguy/ubuntu2004"

    config.ssh.insert_key = false

    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |v|
      v.memory = 384
      v.linked_clone = true
    end

    config.vm.hostname = "geerlingguy-ubuntu2004.test"
    config.vm.network :private_network, ip: "192.168.60.31"
  end

  # RockyLinux 8 Server
  config.vm.define "rockylinux8" do |config|
    config.vm.box = "geerlingguy/rockylinux8"

    config.ssh.insert_key = false

    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |v|
      v.memory = 256
      v.linked_clone = true
    end

    config.vm.hostname = "geerlingguy-rockylinux8.test"
    config.vm.network :private_network, ip: "192.168.60.40"
  end
end
