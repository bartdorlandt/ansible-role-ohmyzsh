# Ohmyzsh
Sets up the ohmyzsh environment with my desired dependencies

## Requirements
- zsh should already be installed.
- No sudo password required

## Role Variables
Available variables are listed below, along with default values (see defaults/main.yml):

    ohmyzsh_plugins: "git zsh-autosuggestions zsh-syntax-highlighting"

Should these plugins be installed as well?

    copy_theme_bartdorlandt: true


## Dependencies
None

## Example Playbook

    - hosts: localhost
      tasks:
        - name: Ohmyzsh
          ansible.builtin.include_role:
            name: bartdorlandt.ohmyzsh

or:

    - hosts: localhost
      roles:
        - role: bartdorlandt.ohmyzsh
          vars:
            use_theme_bart: false
            ohmyzsh_plugins: "git zsh-autosuggestions zsh-syntax-highlighting poetry debian"



## License

MIT/BSD

## Author Information

This role was created in 2022 by Bart Dorlandt.