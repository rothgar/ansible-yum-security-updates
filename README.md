Automatic yum-security updates
==============

This Ansible playbook will automatically install two packages

* yum-cron
* yum-plugin-security (yum-security on rhel5)

It will then configure the packages to run yum updates using the `yum --security update-minimal`
command every morning.

This will also enable install the EPEL repo if you're using RHEL5 or temporarily enable the
rhel-6-server-optional-rpms repo for RHEL6. This will require that you are registered with RedHat.