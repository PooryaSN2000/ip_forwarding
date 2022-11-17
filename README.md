# ip_forwarding

-----------------  Foreign server  -------------------

apt-get update -y && apt-get upgrade -y

apt install curl -y

bash <(curl -Ls https://raw.githubusercontent.com/vaxilu/x-ui/master/install.sh)

x-ui

15
-------------

Panel V2ray :

IP-SERVER:54321

-----------------  The server of your country  -------------------

apt-get update -y && apt-get upgrade -y
sudo apt-get update


sudo apt-get install iptables
sudo iptables -L -v


sysctl net.ipv4.ip_forward=1
iptables -t nat -A PREROUTING -p tcp --dport 22 -j DNAT --to-destination IP_LOCAL_SERVER
iptables -t nat -A PREROUTING -j DNAT --to-destination IP_Foreign_SERVER
iptables -t nat -A POSTROUTING -j MASQUERADE

suggestion :

wget -N --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && bash bbr.sh


-----------------  Check_DNS_SERVER  -------------------

cat /etc/resolv.conf

nano /etc/resolv.conf

nameserver DNS1

nameserver DNS2

Cntrl+X

Y

Enter

-----------------  SPEEDTEST_SERVER  -------------------

sudo apt install speedtest-cli

speedtest-cli --secure

--------------  Check open ports in Linux --------------

sudo netstat -tulpn | grep LISTEN


