
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-24.04"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = 2048
    vb.cpus = 2
    vb.name = "Vagrant_Lab"
  end

  config.vm.network "private_network", ip: "192.168.56.10"

  # Pass cloud-init user-data
  config.vm.cloud_init content_type: "text/cloud-config", path: "cloud-init/user-data"
end