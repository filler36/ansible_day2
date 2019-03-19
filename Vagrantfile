Vagrant.configure("2") do |config|

  config.vm.define "master_node" do |master_node|
    master_node.vm.box = "sbeliakou/centos"
    master_node.vm.hostname = "master-node"
    master_node.vm.network "private_network", ip: "192.168.56.100"
    master_node.vm.provider "virtualbox" do |vb|
      vb.name = "master_node"
      vb.memory = "2048"
    end
  end

  config.vm.define "worker_node" do |worker_node|
    worker_node.vm.box = "sbeliakou/centos"
    worker_node.vm.hostname = "worker-node"
    worker_node.vm.network "private_network", ip: "192.168.56.101"
    worker_node.vm.provider "virtualbox" do |vb|
      vb.name = "worker_node"
      vb.memory = "1048"
    end
  end

end
