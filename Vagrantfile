# -- mode: ruby --
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
 config.vm.define :servidor1 do |servidor1|
 servidor1.vm.provision "shell", path: "servidores.sh.txt"
 servidor1.vm.box = "generic/centos8"
 servidor1.vm.network :private_network, ip: "192.168.50.3"
 servidor1.vm.hostname = "servidor1"
 end
 config.vm.define :servidor0 do |servidor0|
 servidor0.vm.provision "shell", path: "servidores.sh.txt"
 servidor0.vm.box = "generic/centos8"
 servidor0.vm.network :private_network, ip: "192.168.50.4"
 servidor0.vm.hostname = "servidor0"
 end
 config.vm.define :haproxy do |haproxy|
 haproxy.vm.provision "shell", path: "haproxyy.sh.txt"
 haproxy.vm.box = "generic/centos8"
 haproxy.vm.network :private_network, ip: "192.168.50.5"
 haproxy.vm.hostname = "haproxy"
 end
  config.vm.define :servidor3 do |servidor3|
 servidor3.vm.provision "shell", path: "servidores.sh.txt"
 servidor3.vm.box = "generic/centos8"
 servidor3.vm.network :private_network, ip: "192.168.50.6"
 servidor3.vm.hostname = "servidor3"
 end
end
