# frozen_string_literal: true

Vagrant.configure('2') do |config|
  config.vm.box = 'ubuntu/focal64'

  config.vm.provider :virtualbox do |v|
    v.memory = 2048
    v.cpus = 2
  end

  config.vm.synced_folder '.', '/vagrant', type: 'virtualbox'

  config.vm.provision 'ansible_local', run: 'always' do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.galaxy_role_file = 'requirements.yml'
    ansible.galaxy_command = 'ansible-galaxy install --role-file=%{role_file} --roles-path=%{roles_path}'
  end
end
