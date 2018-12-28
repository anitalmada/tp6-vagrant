# -*- mode: ruby -*-
# vi: set ft=ruby :
$script = <<-SCRIPT
sudo apt-get update
sudo apt-get -y install mysql-server
curl -sL https://deb.nodesource.com/setup_11.x | sudo -E bash -
sudo apt-get install -y nodejs
SCRIPT

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.provision "shell", inline: $script

end
