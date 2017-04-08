# Installation
```
 npm i sync-zsh-history -g
```

#Usage
create a file under the synced directory of some cloud storage service, let's say `~/.config/history/.zsh_history`
```
synczshistory ~/.config/history/.zsh_history
```
it will merge `~/.config/history/.zsh_history` and `~/.zsh_history`, remove duplicated commands, and write the results back to them both, then you can merge it in other machine.