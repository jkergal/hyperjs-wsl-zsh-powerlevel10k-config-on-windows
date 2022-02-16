# Configuration to use Hyper.js terminal with WSL on windows 10, zsh and Oh My Zsh / Powerlevel10k theme

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
        `shellArgs: ['~'],`
       
set default path
        `echo "cd ~/path" >> ~/.zshrc`
if your path is in another disk :
        `echo "cd mnt/disk_letter/eventually_a_folder" >> ~/.zshrc`


reinstall node and npm for this shell :
This is for version 16 (view current LTS version):

        `curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -`
        `sudo apt-get install -y nodejs`

Then install build tools so you can install add-ons for npm later

        `sudo apt-get install -y build-essential`
        
Now you can type in

        `npm -v`
        `node -v`
        `Same thing: nodejs -v`


To summarise, edit ~/.profile and change your PATH to this:

        `PATH="$HOME/bin:$HOME/.local/bin:/usr/bin:$PATH"`
