# iptables-script
# To block some abusive IP address or range of IPs, you can use the following iptables rules:
## iptables -I INPUT -s 1.2.3.4 -j DROP
## iptables -I INPUT -s 1.2.0.0/16 -j DROP

# For better readability and maintenance, it is a good idea to have all abusing IPs in one particular file, for example /etc/blacklist.ips. This way, you can add the IP addresses or subnets in this file (one IP or subnet per line) and use the fwall-rules script below to block anything listed in this file.
# Copy and modify fwall-rules.sh to /usr/local/bin/
# chmod +x /usr/local/bin/fwall-rules.sh
# Create /etc/blacklist.ips with IPs you want to block

