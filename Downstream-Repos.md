## How to request updates from downstream packagers


### Arch Linux
1. Search for the package in: https://www.archlinux.org/packages/
2. On the package page find `Flag Package Out-of-Date` link

### Arch Linux User Repository (AUR)
1. Search for the package in: https://aur.archlinux.org
2. On the package page find `Flag Package Out-of-Date` link

### FreeBSD (aka dports)
Open a ticket on their [Bugzilla](https://bugs.freebsd.org/bugzilla/enter_bug.cgi) bugtracker.

### Haiku Ports


### Homebrew
If you're on MacOS use: https://github.com/Homebrew/homebrew-core/blob/master/CONTRIBUTING.md

If not, then find the formula on github, edit the formula (auto-forks for you), make the appropriate changes (change the version number and get the sha256 (use another updated repo to get the the hash or download the program and run `sha256sum`), the submit a PR via github GUI.

### Linuxbrew
See Homebrew

### Mageia Cauldron
Open an issue at https://bugs.mageia.org

### nixpkgs
Open an issue on their [Github repo](https://github.com/NixOS/nixpkgs/)

### vcpkg
C++ Library Manager for Windows, Linux, and MacOS  
Open an issue on their [Github repo](https://github.com/Microsoft/vcpkg)

### Void Linux
Open an issue on their [Github repo](https://github.com/void-linux/void-packages)
