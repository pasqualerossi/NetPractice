<img width="1013" alt="Level 3" src="https://user-images.githubusercontent.com/58959408/175211075-017970f9-e616-4e9a-a136-f2a36ed0145c.png">

### Level 3: Switches

Switches are a means to allow multiple machines/computers to communicate on a local network between eachother. All the submaks don't need to be the same but each IP needs to be in accordance to the highest level submask. e.g. Submask at C1 is the highest determined submask level (/25) and A1 has a preset IP of 104.198.69.125, so C1 and B1 can have IP values between 104.198.69.1 and 104.198.69.126 and still be on the same network.

### Interface C1 IP
- Same numbers as Interface A1, except the last number has to be different.

### Interface B1 IP
- Same numbers as Interface A1, except the last number has to be different number then Interface C1 and Interface A1

### Interface B1 Mask
- Same numbers as Interface C1's Mask

### Interface A1 Mask
- Same numbers as Interface C1's Mask
