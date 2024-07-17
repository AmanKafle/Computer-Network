# How private and public ip work together to solve the problem of ip shortage?
Firstly, Public IP address is a unique ip address provided by the ISP to a client. similarly, Private IP address is address given to each devices which is locally unique but not globally.
So, to solve the problem of the ip shortage, public and private IP is manipulated using a key technology called NAT. NAT stands for Network address translation, it solves the problem by translating the private IP address given to each devices to a public IP address along with the a port numbern when they access anything on internet, such that all devices can access a website on the internet through the same public ip address.


## For example: 

Lets say we have two devices A and B.

Private IP of A: 192.168.1.3

Private IP of B: 192.168.1.4

Public IP: 192.0.2.1


-So when device A wants to access google.com on the internet. 

-first, NAT will translate the private IP to a public IP along with a unique port number such that response can be send to the exact device.

-google.com will respond to public IP, NAT will retanslate the public IP to a Private IP and now device A will recieve the response.
