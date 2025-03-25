# ansible

This is a repository for learning and practising ansible

- ansible all --key-file ~/.ssh/ansible -i inventory -m ping
- ansible all --list-hosts
- ansible all -m gather_facts
- ansible all -m apt -a update_cache=true	Will fail if there is no sudo access
- ansible all -m apt -a update_cache=true --become --ask-become-pass	To do apt get update
- ansible all -m apt -a name=vim-nox --become --ask-become-pass	To install vim

- To run an ansible playbook:
	- ansible-playbook --ask-become-pass <playbook-name>.yml


pre_tasks: runs before any other task is executed in the play
