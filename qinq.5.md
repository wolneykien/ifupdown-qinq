qinq(5) -- Configuration options for Q-in-Q VLANs in `interfaces(5)` file
=========================================================================

SYNOPSIS
--------

    iface eth0.24.371 inet static


DESCRIPTION
-----------

This extension provides support for configuring double-tagged Q-in-Q
VLANs on network interfaces.

Parameters:

  *  `qinq_trunk_iface`:
  The name of the base (raw) network interface. If `name.ID1.ID2`
  scheme is used for the interface name then this parameter is
  redundant but can be used to override the calculated name.
  
  * `qinq_service_vlan`:
  The service VLAN ID. If `name.ID1.ID2` scheme is used for the
  interface name then this parameter is redundant and has no
  effect.
  
  * `qinq_customer_vlan`:
  The customer VLAN ID. If `name.ID1.ID2` scheme is used for the
  interface name then this parameter is redundant and has no effect.
  
  * `qinq_service_iface`:
  The name of the virtual interface to be created for the service VLAN
  ID tag. If `name.ID1.ID2` scheme is used for the interface name then
  this parameter is redundant but can be used to override the
  calculated name.
  
  * `qinq_service_proto`:
  The name of the VLAN protocol to be used when configuring the
  virtual service VLAN interface. The default value is `802.1ad`.
  
  * `qinq_customer_proto`:
  The name of the VLAN protocol to be used when configuring the
  target (customer) virtual VLAN interface. The default value is
  `802.1Q`.


SEE ALSO
--------

`interfaces(5)`
