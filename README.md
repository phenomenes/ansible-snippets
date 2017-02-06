# Ansible snippets

This repo contains snippets for Ansible.

##  Requirements

* [UtilSnips](https://github.com/SirVer/ultisnips) or [SnipMate](https://github.com/garbas/vim-snipmate)
* [vim-plug](https://github.com/junegunn/vim-plug) (optional)

## Installation

To install using [vim-plug](https://github.com/junegunn/vim-plug) add `Plug 'phenomenes/ansible-snippets'`
to you `~/.vimrc` and `:PlugInstall` or `$ vim +PlugInstall +qall`

To install manually clone the repo to your favourite location:

```
$ git clone https://github.com/phenomenes/ansible-snippets.git ~/ansible-snippets
$ cp -r ~/ansible-snippets/* ~/.vim/
```

## Usage

Edit a `.yml` or `.yaml` file, type `play` or any Ansible's module name and use
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

## Credits

This snippets were generated with [ansible_snippet_generator](https://github.com/phenomenes/ansible_snippet_generator)
forked from [bleader/ansible_snippet_generator](https://github.com/bleader/ansible_snippet_generator)
