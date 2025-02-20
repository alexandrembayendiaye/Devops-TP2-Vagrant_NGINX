Vagrant.configure("2") do |config|
 
  config.vm.define "server" do |webserver|
    webserver.vm.box = "ubuntu/xenial64"


    webserver.vm.box_check_update = false


    webserver.vm.network "forwarded_port", guest: 80, host: 82

    webserver.vm.network "forwarded_port", guest: 3306, host: 3306

    webserver.vm.network "private_network", type: "static", ip: "192.168.0.10"


    webserver.vm.synced_folder "./tomcatwebapps-2", "/opt/tomcat/webapps"


    webserver.vm.provider "virtualbox" do |vb|
   
      vb.gui = true
      vb.name = "webserver-tomcat-2"
      vb.memory = "2048"
    end
  end  
end
