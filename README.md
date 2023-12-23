# homeassistant

Various notes about issues encountered with HAOS on a VBox VM:

Autostarting VM on Ubuntu Server
- Ubuntu version of VirtualBox does not include the standard autostart service that comes with the Oracle version
- Workaround: create your own autostart service similar to https://www.paulligocki.com/make-virtual-box-vm-autostart/

DeConz
- 'vboxmanage list usbhost' should show the ConBee stick, if not there might be an issue with the stick/host or most likely vbox installation (perhaps a version mismatch with the vbox-ext-pack)
- a passthrough usb filter is probably needed for the HAOS VM

HAOS VM in a bad state
- HAOS opens port 3389 for RDP connections, can connect to it from Microsoft Remote Desktop (host_ip:3389)
- Most of the time running a standard diagnostic is enough

Permissioning root/vboxusers group etc
- TODO

Various notes encountered as a result of self hosting on a Dell Micro PC:
- micro pc on which this VM was running, ran out of BIOS battery after a power cut! Fortunately, changing the battery is fairly trivial.
