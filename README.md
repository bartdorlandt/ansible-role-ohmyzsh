# Ohmyzsh
Sets up the ohmyzsh environment with my desired dependencies

## Requirements
None

## Role Variables
Available variables are listed below, along with default values (see defaults/main.yml):

    ohmyzsh_plugins: "git zsh-autosuggestions zsh-syntax-highlighting"

Should these plugins be installed as well?

    poetry_plugin: true
    fzf_plugin: true


## Dependencies
None

## Example Playbook

    - hosts: localhost
      tasks:
        - name: Ohmyzsh
          ansible.builtin.include_role:
            name: bartdorlandt.ohmyzsh
            apply:
              tags:
                - ohmyzsh
          tags: ohmyzsh

## License

MIT/BSD

## Author Information

This role was created in 2022 by Bart Dorlandt.