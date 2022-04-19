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
3. `Ctrl-b, d` -> detach session 本來執行的活動還是會繼續進行，想要再次進入可以透過`tmux attach -t 0`其中 0 為 session ID 可以透過 `tmux ls` 來找出 session ID為何
4. `Ctrl-b, c` -> New window 在同一個session中
5. `Ctrl-b, &` -> kill current window
6. `Ctrl-b, [` -> into copy mode 在這模式中讓你可以往前瀏覽之前的content
7. In Copy mode, `Ctrl-r` -> 進入向上search模式，會把一樣的字串標記成黃色，按下Enter後離開search 模式，這時候透過鍵盤的n 來持續search 不同位置的結果。
8. 在tmux 下如何清除 the content of a pane?
    ```
    Ctrl-b
    :clear-history
    ```
9. TBD

## gitconfig
### Install
This will download the data from this repo. and store the data in the file name `.gitconfig` which located in your home directory.
- `wget -O- https://raw.githubusercontent.com/yhkuan/configs/main/gitconfig | cat > ~/.gitconfig`
