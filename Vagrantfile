# _*_ mode: ruby _*_



VAGRANTFILE_API_VERSION = "2"


Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

#configuration generales  des VMs

#  config.vm.box = "geerlingguy/centos7"
  config.vm.box = "hashicorp/bionic64"
#  config.vm.box = "ubuntu/trusty32"
#  config.ssh.insert_key = false
#  config.vm.synced_folder ".","/vagrant", disabled: true
#  config.vm.box = "gbarbieru/xenial" #An Ubuntu 16.04 based image
  config.vm.provider :virtualbox do |v|
     v.gui = true
#     v.memory = 256
#     v.linked_clone = true
  end
  
 config.vm.define "flek" do |app|
    app.vm.hostname = "flek.dev"
    app.vm.network :private_network, ip:"192.168.204.200"
 end
#application serveur1
# config.vm.define "app1" do |app|
#    app.vm.hostname = "orc-app1.dev"
#    app.vm.network :private_network, ip:"192.168.60.4"
# end


#application serveur 2

 #config.vm.define "app2" do |app|
 #   app.vm.hostname = "orc-app2.dev"
 #   app.vm.network :private_network, ip:"192.168.60.5"
 #end

#application serveur3
 
 #config.vm.define "app3" do |app|

#    app.vm.hostname = "orc-app3.dev"
#    app.vm.network :private_network, ip:"192.168.60.6"
# end

####application serveur ubuntu 
#  config.vm.define "LAMP" do |db|
#    db.vm.hostname= "lamp.dev"
#    db.vm.network :private_network, ip:"192.168.60.7"
#  end
end
