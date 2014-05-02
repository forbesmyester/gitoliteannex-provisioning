Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/precise32"
  config.vm.box_url = "http://files.vagrantup.com/precise32.box"
  config.vm.hostname = "gitolite"
  config.vm.network "private_network", ip: "192.168.24.11"
  config.vm.provision :shell, :path => "vagrant-ansible-bootstrap"

  config.vm.provider "virtualbox" do |v|
    v.name = "gitolite"
  end


end
