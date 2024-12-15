## プロンプト変更

.bashrc の末尾に以下を追加

```shell
if [ -f /etc/bash_completion.d/git-prompt ]; then
export PS1='\[\033[01;32m\]\u@\h\[\033[01;34m\] \w\[\033[01;31m\]$(__git_ps1) \n\[\033[01;34m\]\$\[\033[00m\] '
else
export PS1='\[\033[01;32m\]\u@\h\[\033[01;34m\] \w \n\[\033[01;34m\]\$\[\033[00m\] '
fi
```
