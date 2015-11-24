Vagrant.configure("2") do |config|
  config.vm.synced_folder ".", "/vagrant", disabled: true
  config.vm.define "percona001" do |percona001|
  percona001.vm.box = "percona001"
  percona001.vm.box_url = "https://f0fff3908f081cb6461b407be80daf97f07ac418.googledrive.com/host/0BwtuV7VyVTSkUG1PM3pCeDJ4dVE/centos7.box"
  percona001.vm.hostname = "percona001"
  percona001.vm.network :public_network, bridge: "p4p1" ,ip: "192.168.2.170"

  #percona001.timezone.value = "US/Pacific"
  percona001.vm.provider "virtualbox" do |vb|
  #   # Display the VirtualBox GUI when booting the machine
  #  vb.gui = true
  #
  #   # Customize the amount of memory on the VM:
          vb.name = "percona001"
     vb.memory = "1024"
    end
end

end

