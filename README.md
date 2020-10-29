

# WinPack (Windows Packages)
Packages that I need for software development in windows 10. Every command here has to be executed in Powershell UwU

## Chocolatey & Scoop
[Chocolatey](https://chocolatey.org/) and [Scoop](https://github.com/lukesampson/scoop/wiki) basically are kind of package manager for Windows similiar to apt-get/yum/homebrew. It makes managing software easy as fuck

    # PoSH Execution Policy
    Set-ExecutionPolicy AllSigned; Set-ExecutionPolicy RemoteSigned -scope CurrentUser
    
    # choco and scoop
    iwr -useb chocolatey.org/install.ps1 | iex; iwr -useb get.scoop.sh | iex; scoop update; scoop bucket add extras
    
## Neovim
config at [my nvim repo](https://github.com/ahmaddynugroho/nvim)

    scoop install neovim
    
## VSCode
    # It's 90.0MB
    scoop install vscode

    # Must have vscode extensions(prettier, material-icon-theme, colonize, vim, editorconfig, & format-files), then set keybinding for find-jump (I set it to ctrl+;)
    code --install-extension esbenp.prettier-vscode; code --install-extension pkief.material-icon-theme; code --install-extension vmsynkov.colonize; code --install-extension vscodevim.vim; code --install-extension editorconfig.editorconfig; code --install-extension jbockle.jbockle-format-files
    
    # Java Extension Pack
    code --install-extension vscjava.vscode-java-pack
    
    # Python Extension Pack
    code --install-extension donjayamanne.python-extension-pack
    
    # Vetur for Vuejs 
    code --install-extension octref.vetur
    
    # ESLiint
    code --install-extension dbaeumer.vscode-eslint
    
    # Tailwindcss Intellisense
    code --install-extension bradlc.vscode-tailwindcss

## Packages
#### Hyper(60MB)
    scoop install hyper
    # Font-family: "Fira Code"; plugins: ['hyper-oceans16', 'hyper-tabs-enhanced', 'hyper-statusline']
#### Git(50.0MB)
    scoop install git
#### Java(200.0MB) & Intellij IDEA (700.0MB)
    scoop install openjdk idea
#### Python(40.0MB) & PyCharm (300.0MB)
    scoop install python pycharm
    # If you need that damn Anaconda just for it's Jupyter Notebook, just use vscode python extension
#### Nodejs LTS(15.0MB) & YARN(2.0MB)
    scoop install nodejs-lts yarn
#### XAMPP(160.0MB) & Composer(2.0MB)
    scoop bucket add nonportable; scoop install xampp-np composer
#### Dart(150MB) & dart-dev(150MB)
    scoop install dart dart-dev
#### Flutter(160MB)
    scoop bucket add java
    scoop install flutter
    
