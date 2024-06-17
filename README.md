# Demo PI

Merri-bek tech demonstration raspberri pi

## Prerequisites

### A new Raspberry Pi

* Flash the SD card with Ubuntu Server 64bit.
* Be sure to set a hostname for the PI
* Your ssh key on the pi. Eg: `ssh-copy-id -i ~/.ssh/id_ed25519 pi@radish.local`

### Controlling computer

Your development machine should probably run Linux or these instructions will be wrong.

* Install python3
* Install ansible `pip install ansible`
* Optional: Install `ansible-lint` using `sudo apt install ansible-lint`
* Ensure you have a ssh key created

## Setting Up a New Pi

### Setup hosts file

Copy `hosts-example` in this directory to a new file called `hosts`. Replace the capitalized sections with the correct values for your needs.

### Setup house_vars file

Copy `house_vars_example.yml` in this directory to a new file called `house_vars.yml`. Change any values to suit your house.

### Run the ansible playbook

`ansible-playbook run.yml`

## Maintenance

### Run the playbook again anytime

`ansible-playbook run.yml`