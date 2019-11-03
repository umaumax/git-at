# git-at

run git command at any repo

## how to use
```
git at ~/dotfiles/ status
```

## how to install
```
install_path="$HOME/local/bin/git-at"
wget https://raw.githubusercontent.com/umaumax/git-at/master/git-at -O "$install_path"
chmod u+x "$install_path"
```

for zsh completion
```
wget https://raw.githubusercontent.com/umaumax/git-at/master/_git_at -O /usr/local/share/zsh/site-functions
```

## bug
`git at . add --chmod=[tab]`で下記のエラー出力が発生する
```
_git:31: bad output format specification
```
