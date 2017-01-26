Installation:

````
    git clone git://github.com/johntfoster/dotvim.git ~/.vim
````

Create symlinks:

````
    ln -s ~/.vim/vimrc ~/.vimrc
````

Install MacVim for YCM package of Vundle from:

https://github.com/macvim-dev/macvim/releases

Download Vundle.Vim: 

````
mkdir ~/.vim/bundle
git clone git://github.com/VundleVim/Vundle.vim ~/.vim/bundle/Vundle.vim
````

For powerline support, make sure you have `vim` built with `+python` and install
powerline into your Python environment.

````
pip install powerline-status
````


Update Vundle submodule

````
    git submodule init
    git submodule update
````

Update bundles:

````
    :PluginInstall!
````

Or from the command line:

````
    vim +PluginInstall +qall
````

You will need to then follow the installation instructions to build the required
files for `YouCompleteMe` and `command-t`.
