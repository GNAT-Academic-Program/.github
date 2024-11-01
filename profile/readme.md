# GNAT Academic Program

## Contact and Support
- To participate or for any information please reach [Olivier Henley](mailto:henley@adacore.com)

## Join our Discord Server
- https://discord.gg/hNpuxYD4ya

## Learn Ada
- [The official way to learn Ada and SPARK](https://learn.adacore.com/courses/intro-to-ada/index.html)
- [AFTI: Ada For The Impatient (Work-In-Progress)](https://github.com/GNAT-Academic-Program/AFTI/)

## Ada main ressources
- [The Ada/SPARK package manager: Alire](https://alire.ada.dev/)
- [The Ada Forum](https://forum.ada-lang.io/)
- [Awesome-Ada](https://github.com/ohenley/awesome-ada/)

## Capstone Ideas
- [Open-ended list of proposals](https://github.com/GNAT-Academic-Program/capstone_proposals)

## Onboarding instructions

1. Our process has been optimized for and tested exclusively on Linux, specifically Ubuntu 20.04/22.04 LTS.    
2. For the best experience, we advise installing and using Linux (preferably Ubuntu LTS) as your operating system.

### Install Alire, an Ada package manager
#### Linux
- Download and unzip the [Alire 2.0.x Linux zip](https://github.com/alire-project/alire/releases/download/v2.0.2/alr-2.0.2-bin-x86_64-linux.zip)
- Add `where_you_unzipped_alr/bin` to [PATH](https://phoenixnap.com/kb/linux-add-to-path)  
- Verify Alire is found on your path. 
``` 
which alr
```

#### Windows
- Download and execute the [Alire 2.0.x Windows installer](https://github.com/alire-project/alire/releases/download/v2.0.2/alr-2.0.2-installer-x86_64-windows.exe)
- Download and install [Everything](https://www.voidtools.com/Everything-1.4.1.1026.x86-Setup.exe)
- Open Everything. Wait it has finished indexing your drives. Then search for `alr.exe` and copy the path where it's found. 
- Add `where_you_found_alr\bin` to [PATH](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/)
- Verify Alire is found on your Path. 
``` 
where alr
```

#### MacOS
##### AARCH64
- Download and unzip the [Alire 2.0.x MacOS aarch64 zip](https://github.com/alire-project/alire/releases/download/v2.0.2/alr-2.0.2-bin-aarch64-macos.zip)

##### X86_64
- Download and unzip the [Alire 2.0.x MacOS x86_64 zip](https://github.com/alire-project/alire/releases/download/v2.0.2/alr-2.0.2-bin-x86_64-macos.zip)

- Add `where_you_unzipped_alr/bin` to [PATH](https://pimylifeup.com/macos-path-environment-variable/):
```
echo "where_you_unzipped_alr/bin" | sudo tee /etc/paths.d/alr_config > /dev/null
```

- Change the permission of the created file with the following command:
```
sudo chmod 644 /etc/paths.d/alr_config
```

- Update the machine's PATH:    
```
/usr/libexec/path_helper -s
```

- Verify Alire is found on your machine's PATH. 
``` 
where alr
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
sudo apt-get install openocd
```
### (Optional) If you need to delete the GAP index:
```
alr index --del gap
```
