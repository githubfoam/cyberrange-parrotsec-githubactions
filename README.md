# cyberrange-parrotsec-githubactions
[![parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-wf.yml)  

~~~~
      Name                    Command                 State                       Ports                  
---------------------------------------------------------------------------------------------------------
        Name                      Command                State                      Ports                  
-----------------------------------------------------------------------------------------------------------
kali                   /bin/bash                        Up                                                 
metasploitable         /bin/sh                          Up                                                 
owasp-juice-shop       docker-entrypoint.sh npm start   Up         0.0.0.0:3000->3000/tcp,:::3000->3000/tcp
parrotsec-beef         /bin/sh -c /init.sh $@           Up                                                 
parrotsec-bettercap    /bin/sh -c bettercap $@          Up                                                 
parrotsec-core         /bin/sh -c bash $@ /bin/bash     Up                                                 
parrotsec-metasploit   /bin/sh -c /msfconsole-sta ...   Up                                                 
parrotsec-nmap         /bin/sh -c nmap $@               Exit 255                                           
parrotsec-security     /bin/sh -c bash $@               Up                                                 
parrotsec-set          /bin/sh -c setoolkit $@          Up                                                 
parrotsec-sqlmap       /bin/sh -c sqlmap $@             Exit 2                                             
postgresql             docker-entrypoint.sh postgres    Up         0.0.0.0:5432->5432/tcp,:::5432->5432/tcp
webgoat                /bin/sh -c /bin/bash /home ...   Up         8080/tcp, 9090/tcp                       
~~~~

~~~~
https://github.com/ParrotSec/parrot-tools/blob/master/debian/control

parrot-tools-reversing
  Recommends: clang
  Recommends: dex2jar
  Recommends: edb-debugger
  Recommends: gdb
    gdb-minimal
  Recommends: javasnoop
  Recommends: rizin
  Recommends: rizin-cutter
  Recommends: smali
  ~~~~