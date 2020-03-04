BOX_LIMIT=2
Vagrant.configure("2") do |config|
    config.vm.provision "shell", inline: "echo Hello"
    for i in 0..BOX_LIMIT
        config.vm.define "app-#{i}" do |app|
            app.vm.box = "centos/7"
        end
    end
end  