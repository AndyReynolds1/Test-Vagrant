Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/focal64"
  config.vm.network "private_network", ip: "192.168.56.10", netmask: "255.255.255.0"
  config.vm.hostname = "vagrant"

  config.vm.provider "virtualbox" do |vb|
    vb.name = "VagrantTest"
    vb.cpus = "2"
    vb.memory = "2048"
  end

  config.vm.provision "shell", inline: <<-SHELL
    apt-get -y install nginx
    service nginx start
  SHELL

end
