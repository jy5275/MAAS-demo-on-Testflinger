# Deploy MAAS on a testflinger server

[This tutorial](https://maas.io/tutorials/build-a-maas-and-lxd-environment-in-30-minutes-with-multipass-on-ubuntu#1-overview)
guides you to install a demo MAAS cluster on a PC, using Multipass.

However, VMs are resource consuming and personal PC isn't powerful enough to hold them.

We want to use testflinger machine to launch the demo MAAS instead.

This testflinger job is equivalent to step 1-5 in the tutorial above. 
After finish, resume the tutorial from [step 6](https://maas.io/tutorials/build-a-maas-and-lxd-environment-in-30-minutes-with-multipass-on-ubuntu#6-log-into-maas)

```
sudo snap install testflinger-cli
testflinger-cli submit --poll testflinger-maas.yml
```