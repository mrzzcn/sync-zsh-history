# Installation
```
 npm i sync-zsh-history -g
```

# Usage
create a file under the synced directory of some cloud storage service, let's say `~/dropbox/.zsh_history`

```
synczshistory ~/dropbox/.zsh_history
```
it will merge `~/dropbox/.zsh_history` and `~/.zsh_history`, remove duplicated commands, and write the results back to both, then you can merge it in another machine.

# Automatic

```bash
wget https://raw.githubusercontent.com/mrzzcn/sync-zsh-history/master/com.github.mrzzcn.sync-zsh-history.plist

# Before this, you may want to change trigger time and log file location.
launchctl load -w com.github.mrzzcn.sync-zsh-history.plist
```
