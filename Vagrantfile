# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.ssh.insert_key = false
  config.vm.allow_hosts_modification = true
  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
  end

  config.vm.define "test1" do |test1|
  	test1.vm.hostname = "test1"
  	test1.vm.network "private_network", ip: "10.0.0.10"
    test1.vm.provider "virtualbox" do |vb|
      vb.name = "test1"
      vb.memory = 1024
      vb.cpus = 1
	  end
  end

  config.vm.define "test2" do |test2|
  	test2.vm.hostname = "test2"
 	  test2.vm.network "private_network", ip: "10.0.0.11"
    test2.vm.provider "virtualbox" do |vb|
      vb.name = "test2"
      vb.memory = 1024
      vb.cpus = 1
	  end
  end
  
  config.vm.define "test3" do |test3|
  	test3.vm.hostname = "test3"
 	  test3.vm.network "private_network", ip: "10.0.0.12"
    test3.vm.provider "virtualbox" do |vb|
      vb.name = "test3"
      vb.memory = 1024
      vb.cpus = 1
	  end
  end

end
