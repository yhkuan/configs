# configs
My configuration files or resource files to use for work in Linux-based environments.
Minimumm install for development
```
sudo apt install net-tools
sudo apt install openssh-server
- sudo systemctl status ssh (檢查ssh server 是否運行)
sudo apt install tmux
sudo apt install git gitconfig
```

## tmux.conf
### Install
This will download the data from this repo. and store the data in the file name `.tmux.conf` which located in your home directory.
- `wget -O- https://raw.githubusercontent.com/yhkuan/configs/main/tmux.conf | cat > ~/.tmux.conf`
### Features
1. Increase the history to 32768 https://github.com/yhkuan/configs/blob/889000686a927b200c9acbfd160e041b45918bb0/tmux.conf#L2
2. Using `Ctrl-b` then `P` to store the history file from current window. https://github.com/yhkuan/configs/blob/889000686a927b200c9acbfd160e041b45918bb0/tmux.conf#L5
## gitconfig
### Install
This will download the data from this repo. and store the data in the file name `.gitconfig` which located in your home directory.
- `wget -O- https://raw.githubusercontent.com/yhkuan/configs/main/gitconfig | cat > ~/.gitconfig`
