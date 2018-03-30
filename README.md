# ansible-snippets

Ansible Vim snippets for SnipMate and UltiSnips.

## Requirements

* [UtilSnips](https://github.com/SirVer/ultisnips) or [SnipMate](https://github.com/garbas/vim-snipmate)

## Install

To install via [vim-plug](https://github.com/junegunn/vim-plug) add the
following to your `~/.vimrc`

```
Plug 'phenomenes/ansible-snippets'
```

This repo follows [ansible](https://github.com/ansible/ansible)'s `devel`
branch, if you wish to install a previous version you need to specify the tag

```
Plug 'phenomenes/ansible-snippets', { 'tag': 'v2.4.0' }
```

Alternatively you can install it manually by cloning the repo to your `~/.vim`

```
cd ~/.vim/
git clone -b v2.4.0 https://github.com/phenomenes/ansible-snippets.git ~/ansible-snippets
```

## Usage

Open a `.yml` or `.yaml` file, in insert mode type `play` or any Ansible's
module name and press `<tab>` to expand the snippet:

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

Press `<tab>` again to move to the next argument.

## License

BSD 2-clause "Simplified" License
