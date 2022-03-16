### Install Arch 
### https://github.com/yuk7/ArchWSL
`./Arch.exe`

### Setup User
### https://wsldl-pg.github.io/ArchW-docs/How-to-Setup/
```./Arch.exe
passwd
echo "%wheel ALL=(ALL) ALL" > /etc/sudoers.d/wheel
useradd -m -G wheel -s /bin/bash nilson
passwd nilson
exit```

### back to powershell
```./Arch.exe config --default-user nilson
./Arch.exe
curl -fsSL https://raw.githubusercontent.com/nilsonsmf/post-install/master/arch-wsl-post.sh | sudo -E bash -```
