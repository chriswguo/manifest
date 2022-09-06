# manifests

To sync all mango repositories:

1. get the github's ssh(key pairs, token) info and create ~/.ssh
2. install repo from platform's package manager
3. repo init -u git@github.com:chriswguo/manifests.git -m mango.xml <br>
4. repo sync

Note that not all repositories are listed/managed here. <br>
All vim plugin repositories that are managed by "vim plug" are<br>
handled automatically via commands of "vim plug"<br>
e.g.  :PlugInstall, :PlugUpdate, etc. <br>
Those repositories are located at ~/.vim/plugged/

Additiona steps before vim can be used properly: <br>

1. install with platform's package manager(apt, brew): <br>
    fd(fd-find), ripgrep, node <br>
    exuberant(not universal) ctags, just "brew install ctags" on macos <br>
    ccls, which can also be built from source for latest version <br>
2. install bash lanaguage server with "npm i -g bash-language-server" <br>
3. install ccls from platform's package manager(apt,brew) but also can build it for latest version <br>
4. install fzf: <br>
    cd /d/mango/junegunn/fzf/ && ./install <br>
    options during build: <br>
        Do you want to enable fuzzy auto-completion? ([y]/n) -- y <br>
        Do you want to enable key bindings? ([y]/n) -- y <br>
        Do you want to update your shell configuration files? ([y]/n) -- y <br>
5. install autojump: <br>
        cd /d/mango/chriswguo/autojump && ./install <br>
6. source /d/mango/bucket/my_conf/bashrc_append.sh from ~/.bashrc
7. ln -s /d/mango/chriswguo/dot_vim ~/.vim
8. (on mac:) ln -s /opt/homebrew/bin/fd /opt/homebrew/bin/fdfind
9. open basic vim(without loading plugins via gvim or mvim), and run ":PlugInstall"
10. (maybe) /d/mango/chriswguo/dot_vim/coc.config.vim is a copy of README section of
   https://github.com/neoclide/coc.nvim, may need to update when coc.nvim is updated
