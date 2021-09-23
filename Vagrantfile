
Vagrant.configure("2") do |config|

  config.vm.box = "centos/7"

  config.vm.network "forwarded_port", guest: 80, host: 8888
  

  config.vm.synced_folder "shared/", "/home/vagrant/shared/", type: "rsync"

  config.vm.provision "shell", path: "nginx_run.sh"

  
end
