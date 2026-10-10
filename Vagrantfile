Vagrant.configure("2") do |config|
  # Use official Ubuntu Linux 22.04 LTS operating system
  config.vm.box = "ubuntu/jammy64"

  # Configure Virtual Machine: Office Server Node
  config.vm.define "office-server" do |server|
    server.vm.hostname = "office-server"
    server.vm.network "private_network", ip: "192.168.56.10"

    # Set hardware resource limits (1 CPU core, 1024 MB RAM)
    server.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
      v.name = "Office-Server-Node"
    end
  end
end