# ansible-my-linux-workstation

A Ansible playbook that configures a clean install of linux to my preferences.

## Installation

### Quick

1. Run `curl https://raw.githubusercontent.com/justin-p/ansible-my-linux-workstation/master/setup.sh | bash`
2. Enter sudo password.
3. Reboot the system.

### Manual

1. `git clone https://github.com/justin-p/ansible-my-linux-workstation`
2. `cd ansible-my-linux-workstation`
4. `sudo apt-get update -y && sudo apt-get install git curl python3 python3-pip`
5. `pip3 install --user ansible `
6. `export PATH=$PATH:/$HOME/.local/bin`
7. `ansible-galaxy install -r files/requirements.yml`
8. `ansible-playbook main.yml -i inventory.yml`
9. Reboot the system.

## Contributing

Feel free to open issues, contribute and submit your Pull Requests. You can also ping me on Twitter ([@JustinPerdok](https://twitter.com/JustinPerdok))
