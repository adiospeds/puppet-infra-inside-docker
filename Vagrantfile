Vagrant.configure("2") do |config|
 config.vm.box = "bento/ubuntu-16.04"
 config.vm.network "public_network"
 (1..2).each do |i|
  config.vm.define "puppet-client-#{i}" do |node|
  node.vm.hostname = "puppet-client-#{i}.os.com"
  config.vm.provider "virtualbox" do |v|
   v.linked_clone = true
  end
  end
 end
end
