
# WinPack (Windows Packages)
Packages that I need for software development in windows 10. Every command here has to be executed in Powershell UwU

## Chocolatey & Scoop
Chocolatey and Scoop basically is a package manager for Windows similiar to apt-get/yum/homebrew. It makes managing software easy as fuck

    Set-ExecutionPolicy AllSigned
    Set-ExecutionPolicy RemoteSigned -scope CurrentUser
    
    iwr -useb chocolatey.org/install.ps1 | iex
    iwr -useb get.scoop.sh | iex
    scoop bucket add extras
    
## VSCode
    # It's 90.0MB
    scoop install vscode

    # Must have vscode extensions
    code --install-extension esbenp.prettier-vscode vscode-icons-team.vscode-icons vmsynkov.colonize
    
    # Java Extension Pack
    code --install-extension vscjava.vscode-java-pack
    
    # Python Extension Pack
    code --install-extension donjayamanne.python-extension-pack
    
    # Vetur for Vuejs 
    code --install-extension octref.vetur

## Packages
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
    
