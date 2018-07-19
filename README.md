# gitbub-essentials-v2

ls -al ~/.ssh
# Lists the files in your .ssh directory, if they exist

total 12
drwx------  2 dman dman 4096 Jul  6 10:19 .
drwxr-xr-x 57 dman dman 4096 Jul 17 10:23 ..
-rw-r--r--  1 dman dman  884 Jul  6 10:19 known_hosts

ssh-keygen -t rsa -b 4096 -C "douglas.man@me.com"

dman@20B7:/media/dman/Elements/PDF Files$ ssh-keygen -t rsa -b 4096 -C "douglas.man@me.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/home/dman/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/dman/.ssh/id_rsa.
Your public key has been saved in /home/dman/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:BUY/mjTsftCiJ0UjqXHFYlhegzL0bmrsnwnFmoYBOQM douglas.man@me.com
The key's randomart image is:
+---[RSA 4096]----+
|E  ..o.+B        |
|..  +o+*.+       |
|=   .+*.* +      |
| +   * = B .     |
|  . . = S .      |
|   + * + o       |
|  . O o o .      |
|   + . = .       |
|    ..+          |
+----[SHA256]-----+



$ eval "$(ssh-agent -s)"
Agent pid 21873


$ ssh-add ~/.ssh/id_rsa
Identity added: /home/dman/.ssh/id_rsa (/home/dman/.ssh/id_rsa)



dman@20B7:/media/dman/Elements/PDF Files$ ssh-keygen -t rsa -b 4096 -C "douglas.man@me.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/home/dman/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/dman/.ssh/id_rsa.
Your public key has been saved in /home/dman/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:BUY/mjTsftCiJ0UjqXHFYlhegzL0bmrsnwnFmoYBOQM douglas.man@me.com
The key's randomart image is:
+---[RSA 4096]----+
|E  ..o.+B        |
|..  +o+*.+       |
|=   .+*.* +      |
| +   * = B .     |
|  . . = S .      |
|   + * + o       |
|  . O o o .      |
|   + . = .       |
|    ..+          |
+----[SHA256]-----+
dman@20B7:/media/dman/Elements/PDF Files$ eval "$(ssh-agent -s)"
Agent pid 21873
dman@20B7:/media/dman/Elements/PDF Files$ ssh-add ~/.ssh/id_rsa
Identity added: /home/dman/.ssh/id_rsa (/home/dman/.ssh/id_rsa)
dman@20B7:/media/dman/Elements/PDF Files$ sudo apt-get install xclip
[sudo] password for dman: 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  libllvm4.0 libllvm4.0:i386 libllvm5.0 libllvm5.0:i386 libqt4-opengl libuv1 linux-headers-4.4.0-127
  linux-headers-4.4.0-127-generic linux-image-4.4.0-127-generic linux-image-extra-4.4.0-127-generic nodejs
Use 'sudo apt autoremove' to remove them.
The following NEW packages will be installed:
  xclip
0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
Need to get 17.0 kB of archives.
After this operation, 72.7 kB of additional disk space will be used.
Get:1 http://us.archive.ubuntu.com/ubuntu xenial/universe amd64 xclip amd64 0.12+svn84-4 [17.0 kB]
Fetched 17.0 kB in 0s (27.1 kB/s)
Selecting previously unselected package xclip.
(Reading database ... 298493 files and directories currently installed.)
Preparing to unpack .../xclip_0.12+svn84-4_amd64.deb ...
Unpacking xclip (0.12+svn84-4) ...
Processing triggers for man-db (2.7.5-1) ...
Setting up xclip (0.12+svn84-4) ...
dman@20B7:/media/dman/Elements/PDF Files$ xclip -sel clip < ~/.ssh/id_rsa.pub
dman@20B7:/media/dman/Elements/PDF Files$ ssh -T git@gitbub.com
ssh: connect to host gitbub.com port 22: Connection timed out
dman@20B7:/media/dman/Elements/PDF Files$ ssh -T git@gitbub.com
^C
dman@20B7:/media/dman/Elements/PDF Files$ ssh -T git@github.com
Warning: Permanently added the RSA host key for IP address '192.30.253.112' to the list of known hosts.
Hi douglas-man! You've successfully authenticated, but GitHub does not provide shell access.
dman@20B7:/media/dman/Elements/PDF Files$ 

\n## Description\n\n\GitHub for dummies
