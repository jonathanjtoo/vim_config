vim_config
==========

This repository includes mostly vim configuration and environment setup, but it also has stuff like Bash and git profiles.


INSTALLATION
------------

git clone to ~/.vim/

[optional backup all config files]

    mv ~/.vimrc ~/.vimrc_backup
    mv ~/.bashrc ~/.bashrc_backup
    mv ~/.bash_profile ~/.bash_profile_backup
    mv ~/.bash_aliases ~/.bash_aliases_backup
    mv ~/.gitconfig ~/.gitconfig_backup
    mv ~/.gitignore_global ~/.gitignore_global_backup

soft link all config files

    ln -s ~/.vim/dotfiles/.vimrc ~/.vimrc
    ln -s ~/.vim/dotfiles/.bashrc ~/.bashrc
    ln -s ~/.vim/dotfiles/.bash_profile ~/.bash_profile
    ln -s ~/.vim/dotfiles/.bash_aliases ~/.bash_aliases
    ln -s ~/.vim/dotfiles/.gitconfig ~/.gitconfig
    ln -s ~/.vim/dotfiles/.gitignore_global ~/.gitignore_global

install Vundle submodule:

    cd ~/.vim/
    git submodule init && git submodule update

open vim and run Vundle:

    :PluginInstall

additional setups:
    git config --global core.excludesfile ~/.gitignore_global
