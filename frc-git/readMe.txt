
--##########################
Config the git diff 
--##########################
1) Open .gitconfig file. It's located at your home directory: c:\users\username\.gitconfig
2) Add the lines below. Pay attention to the single quotes wrapping the path to winmerge: 

[diff]
    tool = winmerge
[difftool "winmerge"]
    cmd = "'C:/Program Files (x86)/WinMerge/WinMergeU.exe'" -e "$LOCAL" "$REMOTE"

--##########################
Setup - Post-git
--##########################


0) open powershell in administrator mode

1) Set-ExecutionPolicy RemoteSigned

2) Install Nuget provider : 	Install-PackageProvider -Name NuGet –Force
3) Install PowerShellGet : 	Install-Module -Name PowerShellGet –Force
4) Install-Module 	:	Install-Module posh-git -Scope CurrentUser -AllowPrerelease -Force
5) Import-Module	:	Import-Module posh-git	



From <https://github.com/dahlbyk/posh-git#installation> 


https://github.com/kamsiuman/test2.git



