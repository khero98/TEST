# Initialize Raspberry Pi Zero W

## Change the user name
> sudo raspi-config
> sudo adduser dcas_rpi_zero
> sudo usermod -a -G adm,dialout,cdrom,sudo,audio,video,plugdev,games,users,input,netdev,gpio,i2c,spi dcas_rpi_zero
> sudo su - dcas_rpi_zero
> sudo raspi-config
> sudo deluser -remove-home pi

## Setting SSH

> sudo vi /etc/ssh/sshd_config
> systemctl close sshd
> systemctl start sshd
> systemctl start ssh
> systemctl restart sshd
> systemctl enable ssh
> systemctl start ssh
  
##

   49  sudo raspi-config
   50  systemctl start ssh
   51  hostname
   52  hostname -l
   53  hostname -I
   54  sudo iwlist wlan0 scan
   56  sudo vi /etc/wpa_supplicant/wpa_supplicant.conf
   57  sudo reboot
   61  sudo iwlist wlan0 scan
   62  sudo iwlist wlan0 scan ~ grep DCAS
   63  #sudo iwlist wlan0 scan 
   72  sudo raspi-config
   73  sudo dpkg-reconfigure keyboard-configuration
   74  sudo vi /etc/default/keyboard
   75  reboot
   76  systemctl status console-setup.service
   77  sudo vi /etc/default/keyboard
   78  reboot
   79  systemctl status console-setup.service
   80  sudo raspi-config
   81  reboot
   82  history
   83  history 
   84  history 74
   85  sudo vi /etc/default/keyboard
   86  reboot
   87  sudo vi /etc/default/keyboard
   88  reboot
   91  route -n
   92  sudo raspi-config
   93  sudo vi /etc/wpa_supplicant/wpa_supplicant.conf 
   94  sudo rm /etc/wpa_supplicant/wpa_supplicant.conf 
   95  sudo raspi-config
   96  reboot
   97  sudo vi /etc/wpa_supplicant/wpa_supplicant.conf
   99  reboot
  101  sudo vi /etc/wpa_supplicant/wpa_supplicant.conf
  102  reboot
  103  sudo /etc/dhcpcd.conf
  104  dcas
  105  sudo /etc/dhcpcd.conf
  106  sudo vi /etc/dhcpcd.conf
  107  reboot
  109  sudo rm /etc/wpa_supplicant/wpa_supplicant.conf
  110  sudo raspi-config
  111  sudo vi /etc/wpa_supplicant/wpa_supplicant.conf
  112  reboot
  114  sudo vi /etc/wpa_supplicant/wpa_supplicant.conf
  115  reboot
  116  exit
  118  sudo raspi-config
  119  clear
  121  history | grep sshd
  122  sudo vi /etc/ssh/sshd_config
  123  reboote
  124  reboot
  126  cat /etc/wpa_supplicant/wpa_supplicant.conf 
  127  cat /etc/dhcpcd.conf 
  128  ping www.dcas.ac.kr
  129  ping www.naver.com
  130  ping 192.168.0.171
  131  sudo apt-get update && sudo apt-get upgrade -y
  132  bg
  134  bgbg
  135  bg
  136  fg
  137  sudo vim /etc/dhcpcd.conf 
  138  reboot
  139  sudo reboot
  141  sudo apt-get install -y batctl
  142  Reading package lists... Done
  143  Building dependency tree... Done
  144  Reading state information... Done
  145  The following NEW packages will be installed:
  146  0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
  147  Need to get 72.7 kB of archives.
  148  After this operation, 168 kB of additional disk space will be used.
  149  Get:1 http://ftp.kaist.ac.kr/raspbian/raspbian bullseye/main armhf batctl armhf 2020.4-2 [72.7 kB]
  150  Fetched 72.7 kB in 2s (29.7 kB/s)
  151  Selecting previously unselected package batctl.
  152  (Reading database ... 43718 files and directories currently installed.)
  153  Preparing to unpack .../batctl_2020.4-2_armhf.deb ...
  154  Unpacking batctl (2020.4-2) ...
  155  Setting up batctl (2020.4-2) ...
  156  Processing triggers for man-db (2.9.4-2) ...
  157  Reading package lists... Done
  158  Building dependency tree... Done
  159  Reading state information... Done
  160  The following NEW packages will be installed:
  161  0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
  162  Need to get 72.7 kB of archives.
  163  After this operation, 168 kB of additional disk space will be used.
  164  Get:1 http://ftp.kaist.ac.kr/raspbian/raspbian bullseye/main armhf batctl armhf 2020.4-2 [72.7 kB]
  165  Fetched 72.7 kB in 2s (29.7 kB/s)
  166  Selecting previously unselected package batctl.
  167  (Reading database ... 43718 files and directories currently installed.)
  168  Preparing to unpack .../batctl_2020.4-2_armhf.deb ...
  169  Unpacking batctl (2020.4-2) ...
  170  Setting up batctl (2020.4-2) ...
  171  Processing triggers for man-db (2.9.4-2) ...
  172  vim ~/start-batman-adv.sh
  173  ls
  174  chmod +x ~/start-batman-adv.sh 
  175  ls -al
  176  vim ~/start-batman-adv.sh
  177  vim test.cpp
  178  vim .vimrc
  179  vim test.cpp
  180  vim .vimrc
  181  vim test.cpp
  182  vim .vimrc
  183  vim test.cpp
  184  vim .vimrc
  185  vim test.cpp
  186  cat start-batman-adv.sh 
  187  sudo vim /etc/network/interface.d/wlan0
  188  ls /etc/network/interface.d
  189  ls /etc/network/
  190  sudo vim /etc/network/interfaces.d/wlan0
  191  echo 'batman-adv' | sudo tee --append /etc/modules
  192  man tee
  193  echo 'denyinterfaces wlan0' | sudo tee --append \etc
  194  ls /etc/
  195  echo 'denyinterfaces wlan0' | sudo tee --append /etc/dhcpcd.conf 
  196  cat /etc/dhcpcd.conf 
  198  sudo vim /etc/rc.local
  200  cat .vimrc
  201  cat start-batman-adv.sh 
  202  sudo cat /etc/network/interfaces.d/wlan0
  203  history | grep batman-adv
  204  sudo apt-get install -y dnsmasq
  205  sudo vim /etc/dnsmasq.conf
  206  vim start-batman-adv.sh 
  207  sudo reboot
  212  sudo cat /etc/dhcpcd.conf 
  213  sudo vim /etc/dhcpcd.conf 
  214  reboot
  216  ssh 169.254.212.28
  217  ssh 169.254.212.28 308
  218  ssh 169.254.212.28 -p 308
  219  sudo ssh 169.254.212.28 -p 308
  220  ssh 169.254.212.28 -p 308
  223  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  224  sudo cat /etc/network/interfaces.d/wlan0
  225  sudo cat /etc/wpa_supplicant/wpa_supplicant.conf 
  227  sudo reboot
  230  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  231  sudo cat /etc/network/interfaces.d/wlan0
  232  sudo vim /etc/network/interfaces.d/wlan0
  233  sudo reboot
  235  history | grep 168
  236  history | grep 162
  237  history | grep ssh
  238  ssh 169.254.212.28 -p 308
  239  batctl -n
  240  batctl ping
  241  exit
  250  ssh 169.254.116.21
  251  ssh 169.254.116.21 -p 308
  252  ssh 169.254.183.154 -p 308
  253  sudo apt-get install hostapd isc-dhcp-server quuagga
  262  sudo cat /etc/wpa_supplicant/wpa_supplicant.conf 
  263  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  264  reboot
  267  ping 
  268  ping 192.168.199.48
  269  ssh 
  270  history
  271  sudo cat /etc/network/interfaces.d/wlan0
  272  sudo vim /etc/network/interfaces.d/wlan0
  273  sudo cat /etc/wpa_supplicant/wpa_supplicant.conf 
  274  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  275  reboote
  276  reboot
  279  ssh 169.254.118.198 -p 308
  280  lsusb
  281  iw dev
  282  sudo iwlist wlan1 scan
  283  sudo iwlist wlan1 scan | grep ESSID
  284  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  285  reboot
  288  cat start-batman-adv.sh 
  290  sudo batctl if
  291  sudo batctl n
  292  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  293  reboot
  294  exit
  297  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  298  systemctl restart network
  299  systemctl restart networking
  302  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  303  systemctl restart networking
  304  sudo systemctl restart networking
  307  reboot
  308  exit
  311  cat start-batman-adv.sh 
  312  sudo vim /etc/network/interfaces.d/wlan0 
  313  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  314  sudo cat /etc/rc.local
  315  ls
  316  sudo cat /etc/dnsmasq.conf
  317  sudo ls /etc/dnsmasq.d
  318  cat start-batman-adv.sh 
  319  vim start-batman-adv.sh 
  320  systemctl restart networking
  323  ssh dcas_rpi_zero@hostname.local
  324  ssh dcas_rpi_zero@192.168.199.1 -p 308
  326  sudo vim /etc/wpa_supplicant/wpa_supplicant.conf 
  327  sudo systemctl restart networking
  330  sudo cat /etc/dhcpcd.conf 
  332  sudo batctl if
  333  sudo batctl n
  335  reboot
  338  cat st
  339  cat start-batman-adv.sh 
  340  sudo cat /etc/network/interfaces.d/wlan0 
  341  tee -h
  342  tee --help
  343  sudo ls -al /etc | grep modules
  344  sudo cat /etc/modules
  345  sudo cat /etc/dhcpcd.conf 
  346  sudo vim /etc/dhcpcd.conf 
  347  sudo cat /etc/rc.local
  349  sudo systemctl restart networking
  353  cat start-batman-adv.sh 
  354  vim start-batman-adv.sh 
  357  sudo cat /etc/network/interfaces.d/wlan0
  358  sudo batctl if
  359  sudo batctl n
  360  sudo cat /etc/wpa_supplicant/wpa_supplicant.conf 
  363  reboot
  366  sudo cat /etc/dhcpcd.conf 
  367  sudo vim /etc/network/interfaces.d/bat0
  368  sudo systemctl restart networking
  369  reboot
  372  ifconfgi
  375  ping google.com
  376  ping naver.com
  377  ping www.facesbook.com
  378  ping www.gist.ac.kr
  379  reboot
  383  sudo batctl n
  386  sudo batctl if
  387  sudo batctl n
  388  reboot
  391  systemctl status networking.service
  392  sudo rm /etc/network/interfaces.d/bat0
  393  reboot
  396  sudo batctl n
  397  ssh 169.254.3.68 -p 308
  398  ssh dcas_rpi_one@169.254.3.68 -p 308
  399  ssh dcas_rpi_one@192.168.199.19 -p 308
  400  ping www.gist.ac.kr
  401  cat start-batman-adv.sh 
  402  ping www.youtube.com
  403  ping www.github.com
  404  mkdir test && cd test
  405  git clone https://github.com/khero98/TEST.git
  406  cat ../start-batman-adv.sh 
  408  cd .. 
  409  cat start-batman-adv.sh 
  410  sudo cat /etc/dnsmasq.conf 
  411  cat start-batman-adv.sh 
  412  vim start-batman-adv.sh 
  413  sudo sysctl restart networking
  414  reboot
  417  cd test
  418  git clone https://github.com/khero98/TEST.git
  419  ls
  420  rm *
  421  rm -r *
  422  ls
  423  cd TEST
  424  ls
  425  cd ..
  426  rm -d *
  427  rm -rf *
  428  ls
  429  git clone https://github.com/khero98/TEST.git
  430  pnig www.gist.ac.kr
  431  ping www.gist.ac.kr
  432  cd .. 
  433  cat start-batman-adv.sh 
  434  vim start-batman-adv.sh 
  435  fg
  436  /\start-batman-adv.sh 
  437  ./start-batman-adv.sh 
  438  iptables
  439  sudo apt-get install iptables
  440  ./start-batman-adv.sh 
  441  history
  442  mkdir batadv-setting
  443  cd batadv-setting/
  444  git init
  445  git status
  446  history > command-seq.md
