#!/bin/bash
sudo useradd -m apadmin
echo apadmin:redhat123# | sudo chpasswd
sudo usermod -aG wheel apadmin
#sudo cp /tmp/sshd_config /etc/ssh/sshd_config
#echo 'sed -i "/^[^#]*PasswordAuthentication[[:space:]]no/c\PasswordAuthentication yes" /etc/ssh/sshd_config' | sudo tee -a /etc/rc.d/rc.local > /dev/null
#echo 'service sshd restart' | sudo tee -a /etc/rc.d/rc.local > /dev/null
#sudo chmod +x /etc/rc.d/rc.local
sudo sed -i "/^[^#]*PasswordAuthentication[[:space:]]no/c\PasswordAuthentication yes" /etc/ssh/sshd_config
sudo service sshd restart
