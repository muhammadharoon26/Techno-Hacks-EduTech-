# Using the Wireshark Packet Analyzer Tool to Find the ID and Password of the HTTP Website 

1. In Kali Linux open Wireshark program by entering

       sudo wireshark

2. Start Capturing

3. Go to the http login page and enter credentials.

4. Hit enter and comeback to Wireshark

5. Stop Capture

6. Enter the following command on filter

       http.request.method=="POSTS"

7. Hit Enter

8. Search each traffic for HTML Form URL Encoded

9. The encoded form will contain entered credentials.
