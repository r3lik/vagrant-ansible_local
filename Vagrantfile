Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  #config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.hostname = "dev-env.vagrant"
  
  # -= ANSIBLE =-
  # Use :ansible or :ansible_local to provision
  config.vm.provision :ansible_local do |ansible|
    ansible.playbook = "provisioning/site.yml"
    ansible.install_mode = "pip"
    ansible.version = "2.4.2.0"
  end
end
