# Codes for Faults Attacks on Grain-128AEAD

This repository consists of the codes or materials that are used in the experiment of the paper titled _Random Differential Fault Attacks on the Lightweight Authenticated Encryption Stream Cipher Grain-128AEAD_ 

### Codes

1. `Obtaining Output Indices where the Output Differential = 1`
    * This code simulates the Grain-128AEAD cipher and compute the output differential and obtains the list of output indices where the results = 1
    
1. `Getting Unique Output Indices for 16 LFSR Bytes`
    * This code gets the output indices of each byte of registers and obtain the unique output indices (remove duplicated)
    
1. `Get Number of Times of Output Differential = 1 for each Output Indices of Each LFSR Byte`
    * This code obtains the number of times of output differential = 1 for single bit of output index for each LFSR Byte
    
1. `Get Number of Times for Output Differential = 1 for Pairs of Output Indices of Each LFSR Byte`
    * This code obtains the number of times of output differential = 1 for pairs of output index for each LFSR Byte

