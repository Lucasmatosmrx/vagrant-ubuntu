Vagrant.configure("2") do | config |
  config.vm.box = "ubuntu/trusty64"
  config.vm.network = "private_network", ip: "192.168.0.120"
  config.vm.network "shell", inline: "sudo apt update && sudo apt install nginx -y"
  config.vm.provider :virtualbox do |vb|
    vb.memory = "512"
    vb.cpus   = "1"
  end
end