Vagrant.configure("2") do |config|

  config.vm.synced_folder "../../", "/vagrant"

  config.vm.define :ubuntu do |ubuntu|
    ubuntu.vm.box = "generic/ubuntu2204"
    ubuntu.vm.provision "shell",
      inline: "apt-get update && apt-get install -y git expect tmux"
  end
end
