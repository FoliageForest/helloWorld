# 文件操作

## ls

来源: `ls --help`, `man ls`  

Usage: ls [OPTION]... [FILE]...  
List information about the FILEs (the current directory by default).  
Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.  

-a, --all                  do not ignore entries starting with .  
-l                         use a long listing format  
-d, --directory            list directories themselves, not their contents  
-h, --human-readable       with -l and -s, print sizes like 1K 234M 2G etc.  
-r, --reverse                 逆序排列  
-r, --reverse  
              reverse order while sorting  
-t                         sort by modification time, newest first  
-i, --inode                print the index number of each file  
-R, --recursive            list subdirectories recursively  
-F, --classify             append indicator (one of */=>@|) to entries  
-F, --classify[=何时]      指定 <何时> 在项目后追加指示符号（*/=@| 中的一个）  

来源: <https://gnu-linux.readthedocs.io/>

`ls -i [FILE]...` : 查看文件名对应的 inode 号码  

## ssh

ssh -i /root/.ssh/id_rsa root@192.168.8.1

     -i identity_file
             Selects a file from which the identity (private key) for public key authentication is read.
             The default is ~/.ssh/id_dsa, ~/.ssh/id_ecdsa, ~/.ssh/id_ed25519 and ~/.ssh/id_rsa.  Iden‐
             tity files may also be specified on a per-host basis in the configuration file.  It is pos‐
             sible to have multiple -i options (and multiple identities specified in configuration
             files).  If no certificates have been explicitly specified by the CertificateFile directive,
             ssh will also try to load certificate information from the filename obtained by appending
             -cert.pub to identity filenames.
