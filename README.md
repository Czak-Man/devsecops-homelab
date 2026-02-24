# devsecops-homelab
This repo documents my approach to upskill towards a DevSecOps Engineer.

The roadmap is simple and listed here, updating it, whenever needed.

# Setup VMs
Use VirtualBox as a tool.
Both VMs without GUI, server installation only.
SSH config needed from host --> both VMs.

## Setup Ubuntu 24.04 LTS / Rocky9 VM

1. DL the ISO from official Ubuntu page: Ubuntu 24.04 Server
2. Setup QEMU+Virtual Machine packages to run, since atm VirtualBox has issues with dkms and the current Ubuntu Kernel (6.17.0-14-generic).
3. Error while starting virual-machine --> libvirtd permissions missing
     * start virtual-machine with super user (sudo)
4. Move as superuser the images to /var/lib/libvirt/images/
5. Configure the VM
     * 2 vCPU
     * 4 GB RAM
     * 25 GB disk
