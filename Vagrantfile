Vagrant::Config.run do |config|
  config.vm.box       = 'monaqasat'
  config.vm.box_url   = 'http://files.vagrantup.com/precise32.box'
  config.vm.host_name = 'monaqasat.dev'
	
  config.vm.forward_port 3000, 3000
  config.vm.forward_port 5432, 5432

  
  config.vm.provision :puppet,
    :manifests_path => 'puppet/manifests',
    :module_path    => 'puppet/modules'
end
