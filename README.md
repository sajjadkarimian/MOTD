# MOTD 
This is how we can have Message Of the Day In Debian Jessie 


#2)download This Package First : lsb-release python-apt figlet 
<code>sudo apt install lsb-release python-apt figlet </code>

#3)create a directory  /etc/update-motd.d/ if not exists (do backup if directory exists)

#4)Inside this path create this files : 00-header 10-sysinfo 20-update 99-footer

#5)add excute permission to this files 
<code>sudo chmod +x /etc/update-motd.d/*</code> 
#6)remove /etc/motd (if exists) 
#7)create symbolic link : ln -s /var/run/motd /etc/motd  
#8)apt-get -s -o Debug::NoLocking=true upgrade | grep ^Inst | wc -l do this at end 
#9) Use Vim for editor as copying this file into becuase it need to create bash file
 
