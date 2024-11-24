# FortiGate Zero Touch Provisioning  

This playbook aims to streamline a standardised process for utilising Ansible, Ansible
Tower or AWX to provision a FortiGate device within FortiManager ready for Zero Touch
provisioning with FortiZTP.

The Phases of this playbook are the following:

1. Provision a model device utilising a device blueprint into FortiManager
2. Map variables defined within device blueprint to the new created device
3. Push configuration including templated settings to the model device.
4. Push assigned policy package to the device.

After completion, the device is ready to be turned on and provisioned using any ZTP
method available including

- FortiZTP,
- DHCP options 240/241,
- USB Bootstrap,
- Manual light touch provisioning

These may be further automated/added as part of a workflow to string together a complete
provisioning tasks ready for a device to be connected.
