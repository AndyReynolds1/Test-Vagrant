Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/focal64"
  config.vm.network "public_network", ip: "192.168.1.180"
  config.vm.hostname = "master-1"

  config.vm.provider "virtualbox" do |vb|
    
    vb.name = "VagrantTest"
    vb.cpus = "4"
    vb.memory = "4096"
  
  end

  config.vm.provision "shell", path: "bootstrap.sh"

end
