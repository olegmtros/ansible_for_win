# ansible_for_win
entry point is main.yml

commands for that:
standart proggrams enabled by default.
- chrome
- 7zip
- acrobat reader dc

buh options:
- 1c #always install
# need to define version vars cppro_ver=4 or cppro_ver=5
- cryptopro4
- cryptopro5

remote options:
- anydesk
- teamviever
- anyconnect

how to play:
only std:
ansible-playbook main.yml

buh:
ansible-playbook main.yml -e 'buh_prog=true'

buh with crypto4:
ansible-playbook main.yml -e 'buh_prog=true cppro_ver=4'

buh with crypto5:
ansible-playbook main.yml -e 'buh_prog=true cppro_ver=5'

all of them:
ansible-playbook main.yml -e 'buh_prog=true cppro_ver=5 remote_prog= true'
