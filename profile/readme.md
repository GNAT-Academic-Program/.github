# GNAT Academic Program

## Contact and Support
- To participate or for any information please reach [Olivier Henley](mailto:henley@adacore.com)

## Join our Discord Server
- https://discord.gg/hNpuxYD4ya

## Learn Ada
- [The official way to learn Ada and SPARK](https://learn.adacore.com/courses/intro-to-ada/index.html)

## Onboarding instructions

1. Our process has been optimized for and tested exclusively on Linux, specifically Ubuntu 20.04/22.04 LTS.    
2. For the best experience, we advise installing and using Linux (preferably Ubuntu LTS) as your operating system.

### Install Alire, an Ada package manager
- Download and unzip the [Alire 2.0 linux zip](https://github.com/alire-project/alire/releases/download/v2.0.0/alr-2.0.0-bin-x86_64-linux.zip)
- Add `where_you_unzipped/alr` to [PATH](https://phoenixnap.com/kb/linux-add-to-path)  
- Verify Alire is found on your path. 
``` 
which alr
```

### Add the GAP Alire index (IMPORTANT)
The GAP Alire index hosts crates for internal review before public release in the community index. Add this index for access to early crate versions.

From a command line, install the GAP Alire index named `gap` locally:
```
alr index --add git+https://github.com/GNAT-Academic-Program/alire-index --name gap
```
### Install VSCode
```
sudo snap install --classic code
```
### Install the VSCode Ada Extension
```
code --install-extension adacore.ada
```
### Install OpenOCD (needed for embedded)
```
sudo apt-get install opeocd
```
### (Optional) If you need to delete the GAP index:
```
alr index --del gap
```
