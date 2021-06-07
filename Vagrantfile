# frozen_string_literal: true

Vagrant.configure('2') do |config|
  config.vm.box = 'ubuntu/focal64'

  config.vm.provider :virtualbox do |v|
    v.memory = 2048
    v.cpus = 2
  end

  config.vm.synced_folder '.', '/vagrant', type: 'virtualbox'
end
