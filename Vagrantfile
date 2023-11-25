Vagrant.configure("2") do |config|

    config.vm.define "control" do |control|
        control.vm.box = "ubuntu/bionic64"
        control.vm.network "private_network", ip: "192.168.10.12"
        control.vm.hostname = "control"
        control.vm.synced_folder "C:/Users/Sammy/kubernetes_repo/Ansible", "/vagrant_data"
        control.vm.provider "virtualbox" do |vb|
            vb.memory = "1024"
            vb.name = "control"
        end
    end
end