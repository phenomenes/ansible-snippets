# ansible-snippets

Ansible Vim snippets for SnipMate and UltiSnips.

## Requirements

* [UtilSnips](https://github.com/SirVer/ultisnips) or [SnipMate](https://github.com/garbas/vim-snipmate)

## Install

To install via [vim-plug](https://github.com/junegunn/vim-plug) add
`Plug 'phenomenes/ansible-snippets'` to your `~/.vimrc` and `:PlugInstall` or
`$ vim +PlugInstall +qall`

To manually install, clone this repo to your favourite location:

```
$ git clone https://github.com/phenomenes/ansible-snippets.git ~/ansible-snippets
$ cp -r ~/ansible-snippets/* ~/.vim/
```

## Usage

Open a `.yml` or `.yaml` file, in inster mode type `play` or any Ansible's
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

Press `<tab>` again to move between arguments.

## License

BSD 2-clause "Simplified" License
