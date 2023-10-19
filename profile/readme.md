# GNAT Academic Program

## Onboarding instructions

1. Our process has been optimized for and tested exclusively on Linux, specifically Ubuntu 20.04 LTS.    
2. For the best experience, we advise installing and using Linux (preferably Ubuntu LTS) as your operating system.

#### Install Alire, an Ada package manager: 
- Go to https://github.com/alire-project/alire/releases
- Download and unzip the latest linux zip
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

When you are done, you can delete it:
```
alr index --del gap
```