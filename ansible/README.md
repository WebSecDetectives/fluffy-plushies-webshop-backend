### setup ansible env.
Use WSL ubuntu image :


python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install ansible
which ansible

### basic commands

`ansible -u ansible -m ping all -i inventory`

`ansible localhost -m debug -a 'var=groups' -i inventory`

`ansible-playbook -i inventory/hosts.yml site.yml -l faramir-host --list-tasks`


### create passwd entries

use `mkpasswd` to generate hashed credentials