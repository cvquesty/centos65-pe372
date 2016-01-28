This repo holds a stock vagrant implementation for standing up a sample environment.<br>

In the rollup, I have:

CentOS Linux 6.5<br>
Puppet Master with Puppet Enterprise 3.7.2<br>
Puppet Agents 1-3, all customized to the following three environments:<br>
- development<br>
- testing<br>
- production<br>

REQUIRED:
To use this module , you have to install two vagrant plugins:
- vagrant-hosts<br>
- vagrant-pe_build<br>

To install the required plugins, on your local system simply run:

vagrant plugin install vagrant-hosts<br>
vagrant plugin install vagrant-pe_build<br>

To prepare Vagrant to use the included Vagrantfile.

TODO:
- VMWare Fusion Support
  - I have one pull request on VMWare Fusion, and it's a hacky sort of substitute,
    If anyone nows how to get the Vagrantfile to determine the right virtualization
    technology and just "do the right thing" all in one Vagrantfile, that's the 
    "silver bullet" I'm looking for.
