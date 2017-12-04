Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  # Use :ansible or :ansible_local to provision
  config.vm.provision :ansible_local do |ansible|
    ansible.playbook = "provisioning/site.yml"
  end
end
