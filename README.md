# macos-config
# Install

The easiest way to install is to follow the following steps:

Make sure you have signed into the Mac App Store. This makes mas easier to deal with
1. Install Apples's command line tools: xcode-select --install
2. Install Pip: sudo easy_install pip
3. Install Ansible: sudo pip install ansible
4. Clone the Repository: git clone https://github.com/AustinCloudGuru/macos-config
5. Change Directories into the repo: cd mac-playbook
6. Update the requirements file: ansible-galaxy install -r requirements.yml
7. Run the osascript command to account for sandboxing osascript -e 'tell application "Finder"' -e 'set _b to bounds of window of desktop' -e 'end tell'
8. Run the Playbook: ansible-playbook playbook.yml -i inventory -K

Commands:

 xcode-select --install
 sudo easy_install pip
 sudo pip install ansible
 git clone https://github.com/AustinCloudGuru/macos-config
 cd macos-config
 ansible-galaxy install -r requirements.yml
 osascript -e 'tell application "Finder"' -e 'set _b to bounds of window of desktop' -e 'end tell'
 ansible-playbook playbook.yml -i inventory -K
