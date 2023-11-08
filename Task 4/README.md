# Using the Wireshark Packet Analyzer Tool to Find the ID and Password of the HTTP Website 

In Kali Linux open Wireshark program by entering

    sudo wireshark

Start Capturing
Go to the http login page and enter credentials.
Hit enter and comeback to Wireshark
Stop Capture
Enter the following command on filter

    http.request.method=="POSTS"

Hit Enter
Search each traffic for HTML Form URL Encoded
The encoded form will contain entered credentials.
