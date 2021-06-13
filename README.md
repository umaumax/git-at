# git-at

run git command at any repo

You can use `-C ./repo` option! (not this git-at command)

## how to use
``` bash
git at ~/dotfiles/ status
```

## how to install
``` bash
install_path="$HOME/local/bin/git-at"
wget https://raw.githubusercontent.com/umaumax/git-at/master/git-at -O "$install_path"
chmod u+x "$install_path"
```

for zsh completion
``` bash
wget https://raw.githubusercontent.com/umaumax/git-at/master/_git_at -O /usr/local/share/zsh/site-functions
```

## bug
`git at . add --chmod=[tab]`で下記のエラー出力が発生する
``` bash
_git:31: bad output format specification
```

## memo
* 1.8.5 or later: `-C ./repo`
* before 1.8.5: `--git-dir=$PWD/repo/.git --work-tree=$PWD/repo`
