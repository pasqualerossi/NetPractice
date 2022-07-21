<img width="1272" alt="Level 5" src="https://user-images.githubusercontent.com/58959408/175211323-69236723-999e-4327-a8d1-05a6e709a2a4.png">

### Level 5: transfering data through routers

To be able to transfer data through routers, two things need to be taken into consideration.
1. What signals are being sent? (are any signals being filtered)
2. where are these signals being sent to?

(IP-Subnet Mask (filter)) => IP location

If the data is coming from a client, set IP-Subnet Mask to default (will send data to any signal) and IP location as (IP of closest router)

e.g. as R1 has IP of 29.243.205.126 and is closest to A1; client A Routes will be (default => 29.243.205.126), it will be equivalent for R2 and B1.

### Client B: Machine B Routes
- The exact same numbers as Interface R2 IP Numbers.

### Interface B1 IP
- The same numbers as Interface R2 IP, except the last number.

### Interface B1 Mask
- The exact same numbers as Interface R2 Mask Number.

### Interface A1 IP
- The same numbers as Interface R1 IP, except the last number.

### Interface A1 Mask
- The exact same numbers as Interface R1 Mask Numbers.

### Client A: Machine A Routes
- default is the same name that is in Client B: Machine B Routes and the numbers are the exact same numbers in Interface R1 IP.
