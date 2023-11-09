#  Using Nmap to Scan Network for Open Ports and Vulnerable Services

If ip address of website is unknown determine the ip address by entering the following command

    ping <website_URL>

Capture the ip address and scan the network using nmap.

Following format was used for in-depth scanning

    sudo nmap -A -p- -sC -sV -O <ip_address> 
