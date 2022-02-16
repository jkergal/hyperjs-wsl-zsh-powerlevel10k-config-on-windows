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

`        // the shell to run when spawning a new session (i.e. /usr/local/bin/fish)
        // if left empty, your system's login shell will be used by default
        //
        // Windows
        // - Make sure to use a full path if the binary name doesn't work
        // - Remove `--login` in shellArgs
        //
        // Windows Subsystem for Linux (WSL) - previously Bash on Windows
        // - Example: `C:\\Windows\\System32\\wsl.exe`
        //
        // Git-bash on Windows
        // - Example: `C:\\Program Files\\Git\\bin\\bash.exe`
        //
        // PowerShell on Windows
        // - Example: `C:\\WINDOWS\\System32\\WindowsPowerShell\\v1.0\\powershell.exe`
        //
        // Cygwin
        // - Example: `C:\\cygwin64\\bin\\bash.exe`
        shell: 'C:\\Windows\\System32\\wsl.exe',
        // for setting shell arguments (i.e. for using interactive shellArgs: `['-i']`)
        // by default `['--login']` will be used
        shellArgs: ['~'], `
       
set default path
        `echo "cd ~/path" >> ~/.zshrc`
if your path is in another disk :
        `echo "cd mnt/disk_letter/eventually_a_folder" >> ~/.zshrc`
