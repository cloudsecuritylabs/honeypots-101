# honeypots-101

# Configuring HMN on Azure
- create a VM - Ubuntu 18.04
- open ports - 22, 80, 445, 3000, 10000
- install MHN (https://github.com/pwnlandia/mhn)
  - # on Debian or Ubuntu
  - sudo apt install git -y
  - cd /opt/
  - sudo git clone https://github.com/pwnlandia/mhn.git
  - cd mhn/
  - sudo ./install.sh

  
    MHN Configuration

    - Do you wish to run in Debug mode?: y/n n
    - Superuser email: YOUR_EMAIL@YOURSITE.COM
    - Superuser password: 
    - Server base url ["http://1.2.3.4"]: 
    - Honeymap url ["http://1.2.3.4:3000"]:
    - Mail server address ["localhost"]: 
    - Mail server port [25]: 
    - Use TLS for email?: y/n n
    - Use SSL for email?: y/n n
    - Mail server username [""]: 
    - Mail server password [""]: 
    - Mail default sender [""]: 
    - Path for log file ["mhn.log"]: 

- verify services are running (sudo supervisorctl status)
- review ports are open (netstat -tunlp)
- install sensors
- review alerts
