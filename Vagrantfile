Vagrant.configure("2") do |config|
      (1..2).each do |i|
            config.vm.define vm_name="web0#{i}" do |node|
                  node.vm.box = "galindonkov/nginx64"
                  node.vm.hostname = vm_name
                  node.vm.network "forwarded_port", guest: 80, host: 8080 + i
            end
      end
end
