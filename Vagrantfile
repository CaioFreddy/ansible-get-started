Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/trusty64"

  #config.ssh.private_key_path = "chave privada"
  #config.ssh.host = "172.17.177.41"
  #config.ssh.port = 22

  config.vm.define "wordpress" do |m|
	   m.vm.network "private_network", ip: "172.17.177.41"
  end

  config.vm.define "mysql" do |m|
     m.vm.network "private_network", ip: "172.17.177.43"
  end

  config.vm.provider "virtualbox" do |v|
	   v.memory = 1024
  end
end
