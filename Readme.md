My dotfiles, have a look, try them, give me hints for improvement...

Install
=======

    cd ~ && git clone git://github.com/sathishavm/dotfiles.git

Manual Install
--------------
Symlink the files you want to use e.g.

```Bash
cd ~ && ln -s dotfiles/rspec .rspec
```

Automatic install
-----------------

```Bash
curl -L https://raw.github.com/sathishavm/dotfiles/master/autoload.sh | bash -s master
```

it runs `install.rb` which will:

 - *make a backup of all the files it changes* to ~/dotfiles_backup_TIMESTAMP
 - replaces .file through links to dotfiles/file for .bashrc .gitignore .irbrc .rspec
 - replace content of .gitconfig, except for [github] and [user] section

Secret stuff you do not want to share
------
If you add a folder named 'secret' to dotfiles it will also symlink stuff from there.
e.g. `ln -s /home/micha/Dropbox/Private/dotfiles dotfiles/secret`

### [Contributors](http://github.com/sathishavm/dotfiles/contributors)
 - [Roman Heinrich](http://github.com/mindreframer)
 - [Michael Grosser]
