<img width="1149" alt="Level 2" src="https://user-images.githubusercontent.com/58959408/175211021-b75b3b09-bd12-4f01-9f5e-35bcac88e6d3.png">

### Level 2: Understanding Submasks

Submask determine the amount of networks and thereby the number of associated ports available to each network. 
e.g. for client A and client B, A has it's submask preset to 255.255.255.224. 
In binary form is represented as [11111111].[11111111].[11111111].[11100000]. 
This means there are 2^3 networks and for each network, each has 2^5-2 available ports that can be set as routes.
- IPs 196.168.124.225 to 196.168.124.254 are classified as being on the same network if the submask is 255.255.255.224.
- If client A had IP 196.168.124.225 and client B had IP 196.168.124.222, these are not classified as being on the same network.
- The IP can not be the start or end points indicating the networks e.g 196.168.124.223 (end point of network) or 196.168.124.224 (start point of network). 
- With Client D and C: 127.0.0.1 and 127.0.0.4 will not work as these are the LocalHosts, a means of the machine/computer to communicate to itself. IPs 128.0.0.1 and 128.0.0.2 will communicate betweent each other.

For client D the submask is /30, this is short hand for 255.255.255.252 or [11111111].[11111111].[11111111].[11111100] to indicate the amount of 1's in binary form.

Regarding submasks, it's more convenient to set local routes to have the same submask. both client A and client B to have submask: 255.255.255.224

### Interface A1 IP
- Same numbers as Interface B1, except the last number has to be different. 

### Interface B1 Mask
- Make sure the mask number is the same as Interace A1's Mask Number

### Interface C1 IP
- Same numbers as Interface D1 IP, except the last number

### Interface D1 IP
- Same Numbers as Interface C1 IP, except the last number
