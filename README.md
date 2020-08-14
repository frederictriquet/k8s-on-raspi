# k8s-on-raspi

## What I used
- 4 rasperry pies 4 model B with 4 GB of RAM
- each raspi has a 32 GB micro SD card
- Ubuntu 20.04 LTS 64 bits

## Network configuration
I prefered to set static IP addresses through my router setup and leave the raspis request
a "dynamic" IP address.

## Ssh config
- copy public rsa key to each host (into `~ubuntu/.ssh/authorized_keys`)
    >`ssh-copy-id -i ~/.ssh/id_rsa_new.pub ubuntu@raspi1`

> ansible -i hosts.yml all -m ping


- installpubkeys
- log2ram
