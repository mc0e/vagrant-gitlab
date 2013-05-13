
# vagrant-gitlab

This is a fork from https://github.com/mc0e/puppet-gitlab.git, which builds
github from the ground up as a virtual machine using vagrant.

I want to make the github specific part modular so it can be used with a puppet
build alongsideother configuration.

The idea is to split sbadia's project into 3 parts.

* puppet-gitlab will provide only the gitlab specific stuff
* puppet-gitlab_prerequisites will provide all the prerequisites that gitlab
  requires.  If it can be a bit modular that's good.
* vagrant-gitlab will provide a vagrant project which uses the above as sub-projects.

