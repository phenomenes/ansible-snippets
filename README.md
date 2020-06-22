# ansible-snippets

Ansible Vim snippets for SnipMate and UltiSnips.

## Requirements

* [UtilSnips](https://github.com/SirVer/ultisnips) or [SnipMate](https://github.com/garbas/vim-snipmate)

## Install

Depending on what plugin manager you are using, copy the appropiate lines and
use the plugin's install command:

* [Vim-plug](https://github.com/junegunn/vim-plug)

```vim
Plug 'phenomenes/ansible-snippets'
```

* [Vundle](https://github.com/gmarik/vundle)

```vim
Plugin 'phenomenes/ansible-snippets'
```

* [NeoBundle](https://github.com/Shougo/neobundle.vim)

```vim
NeoBundle 'phenomenes/ansible-snippets'
```

* [Pathogen](https://github.com/tpope/vim-pathogen)

```shell
git clone https://github.com/phenomenes/ansible-snippets.git ~/.vim/bundle/terraform-snippets
```

This repo follows [ansible](https://github.com/ansible/ansible)'s `devel`
branch, if you wish to install a different version you need to specify the
corresponding tag.

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
