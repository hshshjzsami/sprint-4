# Objective
Know the port numbers for common application-layer protocols (HTTP/S, FTP, SSH, DNS, RDP).

## Instructor Notes

## Required Resources

## I Do

A port is a destination endpoint for data being transported by TCP or UDP. It completes the destination or origination network address of a message. Here, we're diving into the data link layer. It isn't enough for a packet to be transmit with a destination IP address because at any one time, a device will be running many different tasks.

 TCP would get confused if all packets for all tasks came to the same place. Having unique port numbers for different types of tasks (load a web page vs. transfer a file vs. send an email) ensures that all tasks can be sucessfuly and securely completed. If an IP address represents the street name and city, a port represents the actual house number. 

Well known ports include: 
|Protocol| |Port Number  |
|--|--|--|
| HTTP |Web Pages| 80  |
| HTTPS | Secure Web Pages| 443  |
| FTP |File Transfer| 20 (data), 21 (command)  |
| SSH | 22  |
| DNS | 53  |
| RDP | 3389  |

## We Do
### Example #1
We can access port numbers right in your internet browser. You already know that an URL (like 'google.com') is just shorthand for an IP address. What you may not know, is that the IP address also has a corresponding port. To demonstrate, lets use what we learned above to try to connect to 'google.com' 
1. In your web browser type 'google.com:80', this indicates that you are trying to access google.com's server, at port #80, designated for web pages. Since google.com is indeed a webpage, this should load the google homepage. 
![enter image description here](https://lh3.googleusercontent.com/EAMuSfgyh0YgEerTK7ja2fNMI34RDT6jVZ1VrhXnMO_Rs_APnlwBQBOuHwX0CvWZ2JX0saluozzG)
2. Now try typing 'google.com:443'. This indicates you  are trying to access google.com's server at port #443, designated for *secure* web pages. Should still work, since google.com is a secure webpage. 
![enter image description here](https://lh3.googleusercontent.com/EAMuSfgyh0YgEerTK7ja2fNMI34RDT6jVZ1VrhXnMO_Rs_APnlwBQBOuHwX0CvWZ2JX0saluozzG)
4. Finally, let's try typing in google.com:20, the port number designated for file transfer. You'll get an error message. Why? You're trying to load a web page using a file transfer port. It's like trying to go to your friend Ada's house, but ringing Grace's doorbell. ![enter image description here](https://lh3.googleusercontent.com/EvpwydO-jfWMAz4ybs2169H8lTEFg6V1KYJtxiEr_DIGDPvIHZQX7EryJ-aniY7dTk1FqRKCZU8M)

### Example #2
4. Look at more packet streams in wireshark - screen recording of how to apply column and view all the port numbers in TCP. Most will be 443/some private port.


 

## You Do

## Additional Resources
- Reference: [Well Known Port Numbers](https://www.webopedia.com/quick_ref/portnumbers.asp)
- 

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1NTUxMDkwNTMsLTU2MTc2NDY0Nl19
-->