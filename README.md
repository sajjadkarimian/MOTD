# MOTD
#Message Of the Day In Debian Jessie 
#download This Package First : lsb-release python-apt figlet
#create a directory in this path /etc/update-motd.d/
#Inside this path create this files : 00-header 10-sysinfo 20-update 99-footer
#add excute permission to this files 
#remove /etc/motd
#create symbolic link : ln -s /var/run/motd /etc/motd 
#apt-get -s -o Debug::NoLocking=true upgrade | grep ^Inst | wc -l do this at end
