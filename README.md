# About

A simple example of how to setup a static IP address on the raspberry pi using the `interfaces` file. Assumptions are 
made here so any user should review the configs and modify as needed. This is for SysVInit not SystemD.

# Instructions

```bash
> git clone <repo-url>
> git checkout -b mickledore

# setup build directory, then ...
> bitbake-layers add-layer <layer-name>

# add following to <build-directory/conf/local.conf>
EXTRA_IMAGE_FEATURES:append = " ssh-server-openssh"
```
