# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define :nodo1 do |nodo1|
    nodo1.vm.box = "debian/stretch64"
    nodo1.vm.hostname = "nodo1"
    nodo1.vm.network "private_network", ip: "192.168.5.1",
      virtualbox__intnet: true  
  end

  config.vm.define :nodo2 do |nodo2|
    nodo2.vm.box = "debian/stretch64"
    nodo2.vm.hostname = "nodo2"
    nodo2.vm.network "private_network", ip: "192.168.5.2",  
      virtualbox__intnet: true
  end
  config.vm.provision "ansible" do |ansible|
   ansible.playbook = "playbook.yml"
   ansible.sudo = true
  end
end
