openstack-at-home-ubuntu
========================

Openstack Initial Provisioning at Home with Ubuntu. (Support for Ubuntu 14.04 LTS/trusty, and Openstack Icehouse)


* code by Jioh L. Jung (ziozzang@gmail.com)

* NIC 3ea or 4ea (TODO)
 - eth0: External
 - eth1: MGMT
 - eth2: Private
 - eth3: Storage (TODO)

* Compute
 - nested VMs (with ESXi)
 - NIC : eth1, eth2, eth3
 - nova-compute: using KVM

* Master
 - NIC : eth0, eth1
 - apt repo passthru

* Network
 - NIC : eth0, eth1, eth2

* Block Storage (iSCSI/TODO)


Setup-Controller
================

```
wget -qO- https://raw.githubusercontent.com/ziozzang/openstack-at-home-ubuntu/master/set-controller | bash
```

Setup-Compute
=============

```
wget -qO- https://raw.githubusercontent.com/ziozzang/openstack-at-home-ubuntu/master/set-compute | bash
```

Tip
===

nestedVM option is vhv.enable="true"

