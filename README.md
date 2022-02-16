# hyperjs-wsl-zsh-powerlevel10k-terminal-config

install Windows Subsystem for Linux (WSL) on Microsoft Store (ex: Ubuntu)
install zsh
install oh my zsh
install powerlevel 10k
https://dev.to/vsalbuq/how-to-install-oh-my-zsh-on-windows-10-home-edition-49g2

install fonts and set it on your terminal app (hyperjs) :
https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k


C:\Users\Johann\AppData\Roaming\Hyper
.hyper

around line 95 change to :
        `shell: 'C:\\Windows\\System32\\wsl.exe',`       
around line 95 change to :
        `shellArgs: ['~'],`
       
set default path
        `echo "cd ~/path" >> ~/.zshrc`
if your path is in another disk :
        `echo "cd mnt/disk_letter/eventually_a_folder" >> ~/.zshrc`
