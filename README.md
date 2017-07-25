# MOTD
#1)Message Of the Day In Debian Jessie 
#2)download This Package First : lsb-release python-apt figlet
#3)create a directory in this path /etc/update-motd.d/
#4)Inside this path create this files : 00-header 10-sysinfo 20-update 99-footer
#5)add excute permission to this files 
#6)remove /etc/motd
#7)create symbolic link : ln -s /var/run/motd /etc/motd 
#8)apt-get -s -o Debug::NoLocking=true upgrade | grep ^Inst | wc -l do this at end
#9) Use Vim for editor as copying this file into becuase it need to create bash file
