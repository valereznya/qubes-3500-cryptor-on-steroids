# qvm-3500-lvm-thin-cryptor-on-steroids-with-lusk
The ultimate cryptdevice adventure you can play with Python3, QubesAdmin, IPC and a Flashed TPM 2.0

## requirements
- lvm-thin is part of a lvm-pool of --- blocks on a disk for different VMs, or partitions? what is a LVM
- a QubesAdmin. Qubes.Storage Device abstracts and instruments real /dev/sdb ?
- is that /rw or /system? if sdb is /rw is /sda /system?
- sda1 sdb1 is VM1, sda2 sdb2 is VM2, etc?
- why would the dom0 qproc / admin.Function._respond_ to AppVM rather than AppVM requesting permission on a /dev device, mountpoint

     qvm-block attach <isolated vm> dom0:<disk> in dom0.
  
- dom0 has accesss to disks, <isolated vm> does not. 
- the spec of the mechanism and tool expects fast reversability and reinfliction of encryption, rendering a locked / unlocked state
  
      is the passphrase for cryptsetup passed from dom0 every time using qvm-pass or are we storing the passphrase, how are we prortecting it, sine
      the whole scenario of this being useful is a full system compromization or recovery

- is frequent call of cryptsetup a problem
- implement qvm-cryptor (-d, -e) to obtain permissions with a mutually-exclusive python argparse/parser running in an AppVM  
- add to Qubes Settings and Qube Create in .desktop menu launcher
- find out why legitimate discussoin and negotiation with a guy waving cash and back and forth being nice and a dick leads to removal from Qubes-Issues.
- be less talkative, and find a new OS. QubesOS is starting to suck.
