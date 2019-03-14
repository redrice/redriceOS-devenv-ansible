# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "fedora/29-cloud-base"
  config.vm.provision :ansible do |ansible|
    ansible.extra_vars = { ansible_python_interpreter:"/usr/bin/python3" }
    ansible.playbook = "site.yml"
  end
end

