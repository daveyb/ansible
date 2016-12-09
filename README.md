# daveyb's Ansible Playbook

This is my personal (and always a WIP) Ansible playbook for setting up and enforcing a consistent config on my computers.

It's designed to init new dotfiles as needed, so be aware that it may clobber existing dotfiles you already have.

##Usage
###Prerequisites
1. Python 2.7+ and `pip`
2. A user account that's a member of the sudoers group `adduser <user> sudo`
3. Ansible `sudo pip install ansible`
4. An internet connection

###Clone
`git clone https://github.com/daveyb/ansible.git /usr/local/src && cd /usr/local/src`

###Run all plays
`ansible-playbook -i hosts main.yml --ask-sudo-pass`

###Run a specific play based on tag (optional)
`ansible-playbook -i hosts main.yml --ask-sudo-pass --tags=zsh`

