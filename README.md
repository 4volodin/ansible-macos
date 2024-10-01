## Installation

1. install Command Line Tools
xcode-select --install
2. /usr/sbin/softwareupdate --install-rosetta --agree-to-license

3. Install Ansible
- export PATH="$HOME/Library/Python/3.9/bin:/opt/homebrew/bin:$PATH"
- sudo spctl --master-disable
- sudo pip3 install --upgrade pip
- pip3 install ansible

4. Clone this repo to home dir
5. ansible-galaxy install -r requirements.yml
6. ansible-playbook -c local ansible_osx.yml --ask-become-pass

sudo spctl --master-enable


