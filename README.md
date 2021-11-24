# cyberrange-parrotsec-githubactions
[![parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-wf.yml)  
~~~~
        git clone https://github.com/githubfoam/cyberrange-parrotsec-githubactions.git && cd cyber*
        sudo docker-compose --file dockerfiles/parrotsec/docker-compose-parrotsec-tools-forensic.yml  up -d
        sudo docker-compose --file dockerfiles/parrotsec/docker-compose-parrotsec-tools-forensic.yml  ps        
        docker exec parrotsec-forensic ls
        docker exec parrotsec-forensic  /bin/bash -c "touch a.txt && hashdeep a.txt"
        docker exec parrotsec-forensic  /bin/bash -c "autopsy"
        docker exec parrotsec-forensic  /bin/bash -c "curl http://localhost:9999"

~~~~

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
[![tools-reversing parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-reversing-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-reversing-wf.yml)  
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
[![privacy parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-privacy-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-privacy-wf.yml)
~~~~

https://github.com/ParrotSec/parrot-tools/blob/master/debian/control

2021-11-23T10:41:56.0172783Z [0mparrot-privacy
2021-11-23T10:41:56.0173312Z   Depends: anonsurf
2021-11-23T10:41:56.0173738Z   Depends: tor
2021-11-23T10:41:56.0174446Z   Depends: torbrowser-launcher
2021-11-23T10:41:56.0175152Z   Recommends: ricochet-im
2021-11-23T10:41:56.0175665Z   Recommends: nyx
2021-11-23T10:41:56.0176083Z   Recommends: mat2
2021-11-23T10:41:56.0176713Z   Recommends: anonsurf-gtk
2021-11-23T10:41:56.0177367Z   Recommends: anonsurf-cli
2021-11-23T10:41:56.0177888Z   Recommends: onionshare
2021-11-23T10:41:56.0178530Z   Suggests: parrot-crypto
2021-11-23T10:41:56.0179052Z   Suggests: onioncircuits
~~~~
[![tools-cloud parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-cloud-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-cloud-wf.yml)
~~~~

https://github.com/ParrotSec/parrot-tools/blob/master/debian/control

2021-11-23T10:29:21.6833432Z 
2021-11-23T10:29:21.8305747Z [0mparrot-tools-cloud
2021-11-23T10:29:21.8306544Z   Recommends: aircrack-ng
2021-11-23T10:29:21.8307071Z   Recommends: nginx
2021-11-23T10:29:21.8307655Z     nginx-core
2021-11-23T10:29:21.8308222Z     nginx-extras
2021-11-23T10:29:21.8308793Z     nginx-full
2021-11-23T10:29:21.8309339Z     nginx-light
2021-11-23T10:29:21.8309820Z   Recommends: arping
2021-11-23T10:29:21.8310315Z   Recommends: crunch
2021-11-23T10:29:21.8310796Z   Recommends: davtest
2021-11-23T10:29:21.8311291Z   Recommends: dc3dd
2021-11-23T10:29:21.8311757Z   Recommends: dhcpig
2021-11-23T10:29:21.8312269Z   Recommends: dirb
2021-11-23T10:29:21.8312750Z   Recommends: dirbuster
2021-11-23T10:29:21.8313261Z   Recommends: dmitry
2021-11-23T10:29:21.8313741Z   Recommends: dns2tcp
2021-11-23T10:29:21.8314249Z   Recommends: dnschef
2021-11-23T10:29:21.8314760Z   Recommends: dnsenum
2021-11-23T10:29:21.8315531Z   Recommends: dnsmap
2021-11-23T10:29:21.8316037Z   Recommends: dos2unix
2021-11-23T10:29:21.8316556Z   Recommends: eapmd5pass
2021-11-23T10:29:21.8317091Z   Recommends: enumiax
2021-11-23T10:29:21.8317585Z   Recommends: ethtool
2021-11-23T10:29:21.8318106Z   Recommends: fcrackzip
2021-11-23T10:29:21.8318603Z   Recommends: fping
2021-11-23T10:29:21.8319097Z   Recommends: hashcat
2021-11-23T10:29:21.8319602Z   Recommends: hping3
2021-11-23T10:29:21.8320085Z   Recommends: iaxflood
2021-11-23T10:29:21.8320869Z   Recommends: impacket-scripts
2021-11-23T10:29:21.8321429Z   Recommends: iodine
2021-11-23T10:29:21.8322109Z   Recommends: isr-evilgrade
2021-11-23T10:29:21.8322630Z   Recommends: john
2021-11-23T10:29:21.8323496Z   Recommends: joomscan
2021-11-23T10:29:21.8324026Z   Recommends: laudanum
2021-11-23T10:29:21.8324508Z   Recommends: links
2021-11-23T10:29:21.8324997Z   Recommends: lynis
2021-11-23T10:29:21.8325521Z   Recommends: maskprocessor
2021-11-23T10:29:21.8326076Z   Recommends: medusa
2021-11-23T10:29:21.8326847Z   Recommends: metasploit-framework
2021-11-23T10:29:21.8327471Z   Recommends: miredo
2021-11-23T10:29:21.8328131Z   Recommends: miredo-server
2021-11-23T10:29:21.8328702Z   Recommends: mitmproxy
2021-11-23T10:29:21.8329203Z   Recommends: nasm
2021-11-23T10:29:21.8329671Z   Recommends: nbtscan
2021-11-23T10:29:21.8330172Z   Recommends: ncrack
2021-11-23T10:29:21.8330686Z   Recommends: netdiscover
2021-11-23T10:29:21.8331208Z   Recommends: nikto
2021-11-23T10:29:21.8331666Z   Recommends: nmap
2021-11-23T10:29:21.8332355Z   Recommends: openssh-server
2021-11-23T10:29:21.8333089Z   Recommends: ophcrack-cli
2021-11-23T10:29:21.8333622Z   Recommends: oscanner
2021-11-23T10:29:21.8334122Z   Recommends: p0f
2021-11-23T10:29:21.8334624Z   Recommends: powersploit
2021-11-23T10:29:21.8335263Z   Recommends: proxychains
2021-11-23T10:29:21.8335696Z     proxychains4
2021-11-23T10:29:21.8336147Z   Recommends: proxytunnel
2021-11-23T10:29:21.8336598Z   Recommends: ptunnel
2021-11-23T10:29:21.8337180Z   Recommends: pwnat
2021-11-23T10:29:21.8337650Z   Recommends: crackmapexec
2021-11-23T10:29:21.8338136Z   Recommends: rainbowcrack
2021-11-23T10:29:21.8338604Z   Recommends: reaver
2021-11-23T10:29:21.8339006Z   Recommends: sbd
2021-11-23T10:29:21.8339415Z   Recommends: set
2021-11-23T10:29:21.8339810Z   Recommends: sfuzz
2021-11-23T10:29:21.8340231Z   Recommends: siege
2021-11-23T10:29:21.8340670Z   Recommends: skipfish
2021-11-23T10:29:21.8341108Z   Recommends: smbclient
2021-11-23T10:29:21.8341558Z   Recommends: smbmap
2021-11-23T10:29:21.8342164Z   Recommends: smtp-user-enum
2021-11-23T10:29:21.8342672Z   Recommends: snmpcheck
2021-11-23T10:29:21.8343094Z   Recommends: socat
2021-11-23T10:29:21.8343547Z   Recommends: spiderfoot
2021-11-23T10:29:21.8343986Z   Recommends: sqlmap
2021-11-23T10:29:21.8344425Z   Recommends: ssldump
2021-11-23T10:29:21.8344862Z   Recommends: sslscan
2021-11-23T10:29:21.8345288Z   Recommends: sslsniff
2021-11-23T10:29:21.8345732Z   Recommends: tcpdump
2021-11-23T10:29:21.8346141Z   Recommends: t50
2021-11-23T10:29:21.8346682Z   Recommends: thc-ipv6
2021-11-23T10:29:21.8347246Z   Recommends: thc-ssl-dos
2021-11-23T10:29:21.8347745Z   Recommends: theharvester
2021-11-23T10:29:21.8348243Z   Recommends: traceroute
2021-11-23T10:29:21.8348877Z     inetutils-traceroute
2021-11-23T10:29:21.8349348Z   Recommends: whois
2021-11-23T10:29:21.8349795Z   Recommends: truecrack
2021-11-23T10:29:21.8350241Z   Recommends: udptunnel
2021-11-23T10:29:21.8350904Z   Recommends: unix-privesc-check
2021-11-23T10:29:21.8351417Z   Recommends: webacoo
2021-11-23T10:29:21.8351873Z   Recommends: webshells
2021-11-23T10:29:21.8352340Z   Recommends: websploit
2021-11-23T10:29:21.8352776Z   Recommends: weevely
2021-11-23T10:29:21.8353227Z   Recommends: whatweb
2021-11-23T10:29:21.8353667Z   Recommends: etherwake
2021-11-23T10:29:21.8354119Z   Recommends: wpscan
2021-11-23T10:29:21.8354532Z   Recommends: xprobe
2021-11-23T10:29:21.8355088Z   Recommends: xsser
2021-11-23T10:29:21.8355516Z   Recommends: yersinia
2021-11-23T10:29:21.8356104Z   Recommends: beef-xss
2021-11-23T10:29:21.8356552Z   Recommends: saidar
2021-11-23T10:29:21.8356981Z   Recommends: hexinject
~~~~
[![tools-common parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-common-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-common-wf.yml)
~~~~
2021-11-23T10:30:12.6298571Z [0mparrot-tools-common
2021-11-23T10:30:12.6299684Z   Recommends: aircrack-ng
2021-11-23T10:30:12.6300061Z   Recommends: arping
2021-11-23T10:30:12.6300415Z   Recommends: asleap
2021-11-23T10:30:12.6300744Z   Recommends: doona
2021-11-23T10:30:12.6301080Z   Recommends: bully
2021-11-23T10:30:12.6301407Z   Recommends: chntpw
2021-11-23T10:30:12.6301763Z   Recommends: cowpatty
2021-11-23T10:30:12.6302131Z   Recommends: creddump7
2021-11-23T10:30:12.6302477Z   Recommends: crunch
2021-11-23T10:30:12.6302827Z   Recommends: cymothoa
2021-11-23T10:30:12.6303168Z   Recommends: davtest
2021-11-23T10:30:12.6303510Z   Recommends: dc3dd
2021-11-23T10:30:12.6303833Z   Recommends: dcfldd
2021-11-23T10:30:12.6304185Z   Recommends: ddrescue
2021-11-23T10:30:12.6304543Z   Recommends: dhcpig
2021-11-23T10:30:12.6304884Z   Recommends: dirb
2021-11-23T10:30:12.6305241Z   Recommends: dirbuster
2021-11-23T10:30:12.6305581Z   Recommends: dmitry
2021-11-23T10:30:12.6305929Z   Recommends: dns2tcp
2021-11-23T10:30:12.6306267Z   Recommends: dnschef
2021-11-23T10:30:12.6306625Z   Recommends: dnsenum
2021-11-23T10:30:12.6306967Z   Recommends: dnsrecon
2021-11-23T10:30:12.6307334Z   Recommends: dnstracer
2021-11-23T10:30:12.6307696Z   Recommends: dnswalk
2021-11-23T10:30:12.6308034Z   Recommends: dos2unix
2021-11-23T10:30:12.6308383Z   Recommends: dsniff
2021-11-23T10:30:12.6308736Z   Recommends: eapmd5pass
2021-11-23T10:30:12.6309521Z   Recommends: enumiax
2021-11-23T10:30:12.6310087Z   Recommends: ethtool
2021-11-23T10:30:12.6310761Z   Recommends: ettercap-graphical
2021-11-23T10:30:12.6311238Z   Recommends: fcrackzip
2021-11-23T10:30:12.6311641Z   Recommends: ferret
2021-11-23T10:30:12.6312030Z   Recommends: fierce
2021-11-23T10:30:12.6312411Z   Recommends: foremost
2021-11-23T10:30:12.6312968Z   Recommends: fping
2021-11-23T10:30:12.6313343Z   Recommends: hexinject
2021-11-23T10:30:12.6313895Z   Recommends: hping3
2021-11-23T10:30:12.6314252Z   Recommends: htshells
2021-11-23T10:30:12.6314631Z   Recommends: iaxflood
2021-11-23T10:30:12.6315222Z   Recommends: impacket-scripts
2021-11-23T10:30:12.6315646Z   Recommends: iodine
2021-11-23T10:30:12.6316181Z   Recommends: isr-evilgrade
2021-11-23T10:30:12.6316567Z   Recommends: john
2021-11-23T10:30:12.6316931Z   Recommends: joomscan
2021-11-23T10:30:12.6317469Z   Recommends: laudanum
2021-11-23T10:30:12.6317993Z   Recommends: libnet1-dev
2021-11-23T10:30:12.6318499Z   Recommends: libpcap-dev
2021-11-23T10:30:12.6318874Z   Recommends: links
2021-11-23T10:30:12.6319209Z   Recommends: lynis
2021-11-23T10:30:12.6319570Z   Recommends: maskprocessor
2021-11-23T10:30:12.6319946Z   Recommends: mdk3
2021-11-23T10:30:12.6320271Z   Recommends: medusa
2021-11-23T10:30:12.6320616Z   Recommends: miredo
2021-11-23T10:30:12.6320960Z   Recommends: mitmproxy
2021-11-23T10:30:12.6321513Z   Recommends: nasm
2021-11-23T10:30:12.6321900Z   Recommends: nbtscan
2021-11-23T10:30:12.6322260Z   Recommends: netdiscover
2021-11-23T10:30:12.6322639Z   Recommends: nishang
2021-11-23T10:30:12.6322965Z   Recommends: nmap
2021-11-23T10:30:12.6323537Z   Recommends: openssh-server
2021-11-23T10:30:12.6323936Z   Recommends: oscanner
2021-11-23T10:30:12.6324300Z   Recommends: outguess
2021-11-23T10:30:12.6324633Z   Recommends: p0f
2021-11-23T10:30:12.6325057Z   Recommends: payloadsallthethings
2021-11-23T10:30:12.6325498Z   Recommends: powercat
2021-11-23T10:30:12.6325867Z   Recommends: powersploit
2021-11-23T10:30:12.6326263Z   Recommends: proxychains
2021-11-23T10:30:12.6326611Z     proxychains4
2021-11-23T10:30:12.6326974Z   Recommends: proxytunnel
2021-11-23T10:30:12.6327336Z   Recommends: ptunnel
2021-11-23T10:30:12.6327752Z   Recommends: pwnat
2021-11-23T10:30:12.6328109Z   Recommends: reaver
2021-11-23T10:30:12.6328456Z   Recommends: reglookup
2021-11-23T10:30:12.6328805Z   Recommends: rig
2021-11-23T10:30:12.6329138Z   Recommends: safecopy
2021-11-23T10:30:12.6329482Z   Recommends: sbd
2021-11-23T10:30:12.6329808Z   Recommends: scalpel
2021-11-23T10:30:12.6330153Z   Recommends: sfuzz
2021-11-23T10:30:12.6330499Z   Recommends: shellinabox
2021-11-23T10:30:12.6330865Z   Recommends: siege
2021-11-23T10:30:12.6331405Z   Recommends: sipcrack
2021-11-23T10:30:12.6331767Z   Recommends: sipvicious
2021-11-23T10:30:12.6332140Z   Recommends: skipfish
2021-11-23T10:30:12.6332482Z   Recommends: smbmap
2021-11-23T10:30:12.6333145Z   Recommends: smbclient
2021-11-23T10:30:12.6333778Z   Recommends: smtp-user-enum
2021-11-23T10:30:12.6334386Z   Recommends: snmpcheck
2021-11-23T10:30:12.6334762Z   Recommends: socat
2021-11-23T10:30:12.6335126Z   Recommends: spiderfoot
2021-11-23T10:30:12.6335512Z   Recommends: sqldict
2021-11-23T10:30:12.6335864Z   Recommends: sqlmap
2021-11-23T10:30:12.6336233Z   Recommends: ssldump
2021-11-23T10:30:12.6336588Z   Recommends: sslscan
2021-11-23T10:30:12.6336967Z   Recommends: sslsniff
2021-11-23T10:30:12.6337338Z   Recommends: steghide
2021-11-23T10:30:12.6337865Z   Recommends: t50
2021-11-23T10:30:12.6338210Z   Recommends: tcpxtract
2021-11-23T10:30:12.6338551Z   Recommends: tcpick
2021-11-23T10:30:12.6338900Z   Recommends: tlssled
2021-11-23T10:30:12.6339248Z   Recommends: tcptrace
2021-11-23T10:30:12.6339776Z   Recommends: thc-ipv6
2021-11-23T10:30:12.6340259Z   Recommends: thc-ssl-dos
2021-11-23T10:30:12.6340665Z   Recommends: theharvester
2021-11-23T10:30:12.6341033Z   Recommends: themole
2021-11-23T10:30:12.6341404Z   Recommends: traceroute
2021-11-23T10:30:12.6341947Z     inetutils-traceroute
2021-11-23T10:30:12.6342326Z   Recommends: whois
2021-11-23T10:30:12.6342679Z   Recommends: udptunnel
2021-11-23T10:30:12.6343222Z   Recommends: unix-privesc-check
2021-11-23T10:30:12.6343637Z   Recommends: wce
2021-11-23T10:30:12.6343964Z   Recommends: webacoo
2021-11-23T10:30:12.6344326Z   Recommends: webshells
2021-11-23T10:30:12.6344700Z   Recommends: websploit
2021-11-23T10:30:12.6345058Z   Recommends: weevely
2021-11-23T10:30:12.6345418Z   Recommends: whatweb
2021-11-23T10:30:12.6345762Z   Recommends: wireshark
2021-11-23T10:30:12.6346135Z   Recommends: etherwake
2021-11-23T10:30:12.6346479Z   Recommends: wpscan
2021-11-23T10:30:12.6346826Z   Recommends: xprobe
2021-11-23T10:30:12.6347162Z   Recommends: xsser
2021-11-23T10:30:12.6347512Z   Recommends: yersinia
2021-11-23T10:30:12.6347870Z   Recommends: zaproxy
2021-11-23T10:30:12.6348216Z   Recommends: zulucrypt
2021-11-23T10:30:12.6348578Z   Recommends: ftester
2021-11-23T10:30:12.6348911Z   Recommends: smali
2021-11-23T10:30:12.6349244Z   Recommends: geany
2021-11-23T10:30:12.6349588Z   Recommends: soundmodem
2021-11-23T10:30:12.6349962Z   Recommends: minimodem
~~~~
[![tools-forensic parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-forensic-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-forensic-wf.yml)
~~~~
2021-11-23T10:29:14.6424588Z [0mparrot-tools-forensic
2021-11-23T10:29:14.6425542Z   Recommends: afflib-tools
2021-11-23T10:29:14.6426069Z   Recommends: dumpzilla
2021-11-23T10:29:14.6426562Z   Recommends: extundelete
2021-11-23T10:29:14.6427049Z   Recommends: rifiuti
2021-11-23T10:29:14.6427650Z   Recommends: ewf-tools
2021-11-23T10:29:14.6428140Z   Recommends: cabextract
2021-11-23T10:29:14.6428618Z   Recommends: autopsy
2021-11-23T10:29:14.6429053Z   Recommends: binwalk
2021-11-23T10:29:14.6429514Z   Recommends: sleuthkit
2021-11-23T10:29:14.6429952Z   Recommends: dc3dd
2021-11-23T10:29:14.6430389Z   Recommends: dcfldd
2021-11-23T10:29:14.6430860Z   Recommends: ddrescue
2021-11-23T10:29:14.6431327Z   Recommends: dex2jar
2021-11-23T10:29:14.6431784Z   Recommends: foremost
2021-11-23T10:29:14.6432299Z   Recommends: galleta
2021-11-23T10:29:14.6432753Z   Recommends: gtkhash
2021-11-23T10:29:14.6433191Z   Recommends: guymager
2021-11-23T10:29:14.6435414Z   Recommends: hashdeep
2021-11-23T10:29:14.6436194Z   Recommends: magicrescue
2021-11-23T10:29:14.6437269Z   Recommends: missidentify
2021-11-23T10:29:14.6438118Z   Recommends: pasco
2021-11-23T10:29:14.6439913Z   Recommends: pdf-parser
2021-11-23T10:29:14.6441388Z   Recommends: pdfid
2021-11-23T10:29:14.6442405Z   Recommends: pev
2021-11-23T10:29:14.6443740Z   Recommends: recoverjpeg
2021-11-23T10:29:14.6444273Z   Recommends: reglookup
2021-11-23T10:29:14.6444794Z   Recommends: regripper
2021-11-23T10:29:14.6445442Z   Recommends: rifiuti2
2021-11-23T10:29:14.6446389Z   Recommends: safecopy
2021-11-23T10:29:14.6447816Z   Recommends: scalpel
2021-11-23T10:29:14.6449014Z   Recommends: scrounge-ntfs
2021-11-23T10:29:14.6450251Z   Recommends: vinetto
2021-11-23T10:29:14.6451064Z   Recommends: xplico
2021-11-23T10:29:14.6451519Z   Recommends: inetsim
2021-11-23T10:29:14.6452198Z   Recommends: forensic-artifacts
2021-11-23T10:29:14.6452892Z   Recommends: gpp-decrypt
2021-11-23T10:29:14.6453419Z   Recommends: smartmontools
2021-11-23T10:29:14.6453901Z   Recommends: yara
~~~~
[![tools-maintain parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-maintain-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-maintain-wf.yml)
~~~~
2021-11-23T10:23:40.2342282Z [0mparrot-tools-maintain
2021-11-23T10:23:40.2343157Z   Recommends: ncat-w32
2021-11-23T10:23:40.2343676Z   Recommends: powercat
2021-11-23T10:23:40.2344180Z   Recommends: dns2tcp
2021-11-23T10:23:40.2344673Z   Recommends: hyperion
2021-11-23T10:23:40.2345172Z   Recommends: iodine
2021-11-23T10:23:40.2345669Z   Recommends: laudanum
2021-11-23T10:23:40.2346147Z   Recommends: nishang
2021-11-23T10:23:40.2346671Z   Recommends: proxychains
2021-11-23T10:23:40.2347162Z     proxychains4
2021-11-23T10:23:40.2347668Z   Recommends: proxytunnel
2021-11-23T10:23:40.2348184Z   Recommends: ptunnel
2021-11-23T10:23:40.2348671Z   Recommends: pwnat
2021-11-23T10:23:40.2349122Z   Recommends: sbd
2021-11-23T10:23:40.2349606Z   Recommends: <shellter>
2021-11-23T10:23:40.2350115Z   Recommends: socat
2021-11-23T10:23:40.2350564Z   Recommends: sslh
2021-11-23T10:23:40.2351048Z   Recommends: stunnel4
2021-11-23T10:23:40.2351550Z   Recommends: udptunnel
2021-11-23T10:23:40.2352059Z   Recommends: webacoo
2021-11-23T10:23:40.2352549Z   Recommends: weevely
2021-11-23T10:23:40.2353290Z   Recommends: windows-binaries
2021-11-23T10:23:40.2353859Z   Recommends: webshells
~~~~
[![tools-password parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-password-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-password-wf.yml)
~~~~
2021-11-23T10:28:05.4987043Z [0mparrot-tools-password
2021-11-23T10:28:05.4987732Z   Recommends: brutespray
2021-11-23T10:28:05.4988230Z   Recommends: cewl
2021-11-23T10:28:05.4988699Z   Recommends: changeme
2021-11-23T10:28:05.4989190Z   Recommends: chntpw
2021-11-23T10:28:05.4989657Z   Recommends: cmospwd
2021-11-23T10:28:05.4990142Z   Recommends: crackle
2021-11-23T10:28:05.4990603Z   Recommends: crunch
2021-11-23T10:28:05.4991094Z   Recommends: fcrackzip
2021-11-23T10:28:05.4991590Z   Recommends: hashcat
2021-11-23T10:28:05.4992044Z   Recommends: hashid
2021-11-23T10:28:05.4992543Z   Recommends: hydra
2021-11-23T10:28:05.4992984Z   Recommends: john
2021-11-23T10:28:05.4993445Z   Recommends: johnny
2021-11-23T10:28:05.4994118Z   Recommends: pack
2021-11-23T10:28:05.4994571Z   Recommends: medusa
2021-11-23T10:28:05.4995044Z   Recommends: onesixtyone
2021-11-23T10:28:05.4996558Z   Recommends: ophcrack-cli
2021-11-23T10:28:05.4997076Z   Recommends: ophcrack
2021-11-23T10:28:05.4997542Z   Recommends: pdfcrack
2021-11-23T10:28:05.4998188Z   Recommends: pipal
2021-11-23T10:28:05.4998662Z   Recommends: pixiewps
2021-11-23T10:28:05.4999194Z   Recommends: rainbowcrack
2021-11-23T10:28:05.4999700Z   Recommends: rarcrack
2021-11-23T10:28:05.5000773Z   Recommends: rcracki-mt
2021-11-23T10:28:05.5001296Z   Recommends: rsmangler
2021-11-23T10:28:05.5001785Z   Recommends: samdump2
2021-11-23T10:28:05.5002442Z   Recommends: sipcrack
2021-11-23T10:28:05.5003154Z   Recommends: sucrack
2021-11-23T10:28:05.5003862Z   Recommends: thc-pptp-bruter
2021-11-23T10:28:05.5004424Z   Recommends: truecrack
2021-11-23T10:28:05.5004911Z   Recommends: twofi
2021-11-23T10:28:05.5005381Z   Recommends: wordlists
2021-11-23T10:28:05.5006084Z   Recommends: device-pharmer
2021-11-23T10:28:05.5006689Z   Recommends: statsprocessor
~~~~
[![tools-postexploit parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-postexploit-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-postexploit-wf.yml)
~~~~
2021-11-23T10:28:24.3954151Z [0mparrot-tools-postexploit
2021-11-23T10:28:24.3955355Z   Recommends: mimikatz
2021-11-23T10:28:24.3956322Z   Recommends: powersploit
2021-11-23T10:28:24.3957681Z   Recommends: passing-the-hash
2021-11-23T10:28:24.3958666Z   Recommends: wce
2021-11-23T10:28:24.3959991Z   Recommends: xspy
2021-11-23T10:28:24.3960816Z   Recommends: lynis
2021-11-23T10:28:24.3962245Z   Recommends: linux-exploit-suggester
~~~~
[![tools-pwn parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-pwn-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-pwn-wf.yml)
~~~~
2021-11-23T10:29:05.5028418Z [0mparrot-tools-pwn
2021-11-23T10:29:05.5029094Z   Recommends: armitage
2021-11-23T10:29:05.5029731Z   Recommends: beef-xss
2021-11-23T10:29:05.5030215Z   Recommends: commix
2021-11-23T10:29:05.5030818Z   Recommends: thc-ipv6
2021-11-23T10:29:05.5031499Z   Recommends: jsql-injection
2021-11-23T10:29:05.5032185Z   Recommends: king-phisher
2021-11-23T10:29:05.5032703Z   Recommends: mdbtools
2021-11-23T10:29:05.5033446Z   Recommends: metasploit-framework
2021-11-23T10:29:05.5034031Z   Recommends: oscanner
2021-11-23T10:29:05.5034510Z   Recommends: pompem
2021-11-23T10:29:05.5034958Z   Recommends: set
2021-11-23T10:29:05.5035427Z   Recommends: shellnoob
2021-11-23T10:29:05.5035929Z   Recommends: sidguesser
2021-11-23T10:29:05.5036455Z   Recommends: sqlmap
2021-11-23T10:29:05.5036928Z   Recommends: websploit
2021-11-23T10:29:05.5037599Z   Recommends: unicorn-magic
2021-11-23T10:29:05.5038366Z   Recommends: backdoor-factory
~~~~
[![tools-sniff parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-sniff-wf%20.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-sniff-wf%20.yml)
~~~~
2021-11-23T10:26:59.9156220Z [0mparrot-tools-sniff
2021-11-23T10:26:59.9157160Z   Recommends: bettercap
2021-11-23T10:26:59.9157616Z   Recommends: chaosreader
2021-11-23T10:26:59.9158193Z   Recommends: darkstat
2021-11-23T10:26:59.9158594Z   Recommends: dnschef
2021-11-23T10:26:59.9159174Z   Recommends: dsniff
2021-11-23T10:26:59.9159574Z   Recommends: sniffjoke
2021-11-23T10:26:59.9160149Z   Recommends: tcpflow
2021-11-23T10:26:59.9160679Z     tcpflow-nox
2021-11-23T10:26:59.9161074Z   Recommends: driftnet
2021-11-23T10:26:59.9161478Z   Recommends: etherape
2021-11-23T10:26:59.9162455Z   Recommends: ettercap-graphical
2021-11-23T10:26:59.9163224Z   Recommends: thc-ipv6
2021-11-23T10:26:59.9163642Z   Recommends: fiked
2021-11-23T10:26:59.9164453Z   Recommends: hamster-sidejack
2021-11-23T10:26:59.9164952Z   Recommends: hexinject
2021-11-23T10:26:59.9165724Z   Recommends: isr-evilgrade
2021-11-23T10:26:59.9166340Z   Recommends: mitmproxy
2021-11-23T10:26:59.9167253Z   Recommends: netsniff-ng
2021-11-23T10:26:59.9168181Z   Recommends: rebind
2021-11-23T10:26:59.9168627Z   Recommends: responder
2021-11-23T10:26:59.9169227Z   Recommends: sslsniff
2021-11-23T10:26:59.9169629Z   Recommends: sslsplit
2021-11-23T10:26:59.9170210Z   Recommends: tcpreplay
2021-11-23T10:26:59.9171109Z   Recommends: wifi-honey
2021-11-23T10:26:59.9171580Z   Recommends: wireshark
2021-11-23T10:26:59.9171977Z   Recommends: yersinia
~~~~
[![tools-vuln parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-vuln-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-vuln-wf.yml)
~~~~
2021-11-23T10:27:11.3788211Z [0mparrot-tools-vuln
2021-11-23T10:27:11.3788804Z   Recommends: afl
2021-11-23T10:27:11.3789253Z   Recommends: doona
2021-11-23T10:27:11.3790151Z   Recommends: thc-ipv6
2021-11-23T10:27:11.3790637Z   Recommends: dhcpig
2021-11-23T10:27:11.3791125Z   Recommends: enumiax
2021-11-23T10:27:11.3791602Z   Recommends: gvm
2021-11-23T10:27:11.3792060Z   Recommends: iaxflood
2021-11-23T10:27:11.3792580Z   Recommends: inviteflood
2021-11-23T10:27:11.3793096Z   Recommends: dsniff
2021-11-23T10:27:11.3793597Z   Recommends: ohrwurm
2021-11-23T10:27:11.3794256Z   Recommends: protos-sip
2021-11-23T10:27:11.3794770Z   Recommends: rtpbreak
2021-11-23T10:27:11.3795274Z   Recommends: rtpflood
2021-11-23T10:27:11.3795810Z   Recommends: rtpinsertsound
2021-11-23T10:27:11.3796393Z   Recommends: rtpmixsound
2021-11-23T10:27:11.3796912Z   Recommends: sipp
2021-11-23T10:27:11.3797818Z   Recommends: slowhttptest
2021-11-23T10:27:11.3798354Z   Recommends: spike
2021-11-23T10:27:11.3798837Z   Recommends: sipvicious
2021-11-23T10:27:11.3799536Z   Recommends: thc-ssl-dos
2021-11-23T10:27:11.3800266Z   Recommends: unix-privesc-check
2021-11-23T10:27:11.3800883Z   Recommends: voiphopper
2021-11-23T10:27:11.3801402Z   Recommends: yersinia
2021-11-23T10:27:11.3801931Z   Recommends: siparmyknife
2021-11-23T10:27:11.3802460Z   Recommends: sctpscan
2021-11-23T10:27:11.3803086Z   Recommends: cisco-ocs
2021-11-23T10:27:11.3803743Z   Recommends: cisco-torch
2021-11-23T10:27:11.3804466Z   Recommends: copy-router-config
~~~~
[![tools-web parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-web-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-web-wf.yml)
~~~~
2021-11-23T10:27:45.4750758Z [0mparrot-tools-web
2021-11-23T10:27:45.4751467Z   Recommends: burpsuite
2021-11-23T10:27:45.4752112Z   Recommends: commix
2021-11-23T10:27:45.4752587Z   Recommends: davtest
2021-11-23T10:27:45.4753040Z   Recommends: dirb
2021-11-23T10:27:45.4753487Z   Recommends: dirbuster
2021-11-23T10:27:45.4753968Z   Recommends: gobuster
2021-11-23T10:27:45.4754572Z   Recommends: joomscan
2021-11-23T10:27:45.4755388Z   Recommends: jsql-injection
2021-11-23T10:27:45.4756236Z   Recommends: nikto
2021-11-23T10:27:45.4756659Z   Recommends: padbuster
2021-11-23T10:27:45.4757113Z   Recommends: skipfish
2021-11-23T10:27:45.4757526Z   Recommends: wfuzz
2021-11-23T10:27:45.4757949Z   Recommends: whatweb
2021-11-23T10:27:45.4758348Z   Recommends: wig
2021-11-23T10:27:45.4758762Z   Recommends: wpscan
2021-11-23T10:27:45.4759350Z   Recommends: xsser
2021-11-23T10:27:45.4759795Z   Recommends: zaproxy
2021-11-23T10:27:45.4760237Z   Recommends: wafw00f
2021-11-23T10:27:45.4760668Z   Recommends: parsero
~~~~
[![tools-wireless parrotsec cyberrange CI workflow](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-wireless-wf.yml/badge.svg?branch=main)](https://github.com/githubfoam/cyberrange-parrotsec-githubactions/actions/workflows/parrotsec-tools-wireless-wf.yml)
~~~~
2021-11-23T10:30:59.4598783Z [0mparrot-tools-wireless
2021-11-23T10:30:59.4599543Z   Recommends: aircrack-ng
2021-11-23T10:30:59.4600025Z   Recommends: airgeddon
2021-11-23T10:30:59.4600483Z   Recommends: asleap
2021-11-23T10:30:59.4600917Z   Recommends: bluelog
2021-11-23T10:30:59.4601355Z   Recommends: blueranger
2021-11-23T10:30:59.4601836Z   Recommends: bluesnarfer
2021-11-23T10:30:59.4602289Z   Recommends: btscanner
2021-11-23T10:30:59.4602904Z   Recommends: bluez-hcidump
2021-11-23T10:30:59.4603354Z   Recommends: bully
2021-11-23T10:30:59.4603778Z   Recommends: cowpatty
2021-11-23T10:30:59.4604220Z   Recommends: crackle
2021-11-23T10:30:59.4604663Z   Recommends: eapmd5pass
2021-11-23T10:30:59.4605323Z   Recommends: fern-wifi-cracker
2021-11-23T10:30:59.4605803Z   Recommends: hackrf
2021-11-23T10:30:59.4606250Z   Recommends: inspectrum
2021-11-23T10:30:59.4606834Z   Recommends: king-phisher
2021-11-23T10:30:59.4607284Z   Recommends: mdk3
2021-11-23T10:30:59.4607674Z   Recommends: mfcuk
2021-11-23T10:30:59.4608080Z   Recommends: mfoc
2021-11-23T10:30:59.4608490Z   Recommends: mfterm
2021-11-23T10:30:59.4609078Z   Recommends: libfreefare-bin
2021-11-23T10:30:59.4610057Z   Recommends: libnfc-bin
2021-11-23T10:30:59.4610527Z   Recommends: pixiewps
2021-11-23T10:30:59.4610966Z   Recommends: reaver
2021-11-23T10:30:59.4611381Z   Recommends: redfang
2021-11-23T10:30:59.4611801Z   Recommends: rfcat
2021-11-23T10:30:59.4612430Z   Recommends: rtlsdr-scanner
2021-11-23T10:30:59.4613221Z   Recommends: ubertooth
2021-11-23T10:30:59.4613819Z   Recommends: wifi-honey
2021-11-23T10:30:59.4614248Z   Recommends: wifite
2021-11-23T10:30:59.4614680Z   Recommends: yersinia
~~~~