# Ansible snippets

This repo contains snippets for Ansible.

##  Requirements

* [UtilSnips](SirvVer/ultisnips) or [SnipMate](garbas/vim-snipmate)
* [vim-plug](junegunn/vim-plug) (optional)

## Installation

To install using [vim-plug](junegunn/vim-plug):

```
" add this line to your .vimrc
Plug 'phenomenes/ansible-snippets'
```

To install manually, clone the repo:

```
cp -r /<repo_path>/ansible-snippets/* ~/.vim/
```

## Usage

Edit a `.yml` or `.yaml` file, type `play` or an Ansible module name and use
`<tab>` to expand the snippet:

```
- hosts: group
  user: root
  tasks:

- name: task_description
  ec2:
    image: None
    instance_type: None
    #kernel:
    #monitoring:
    #user_data:
    #termination_protection:
    #private_ip:
    #spot_type: one-time
    #ec2_url:
    #id:
    #source_dest_check: True
    #aws_secret_key:
    #spot_wait_timeout: 600
    ...
```

Use `<tab>` again to move between arguments.

