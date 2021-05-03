# Codes for Faults Attacks on Grain-128AEAD

This repository consists of the codes or materials that are used in the experiment of the paper titled **_Random Differential Fault Attacks on the Lightweight Authenticated Encryption Stream Cipher Grain-128AEAD_** 

The experiments were done using [SageMath](https://www.sagemath.org/). 

### Codes

1. `ANF generation and diff with respect to S` and `ANF generation and diff with respect to B`
    * Generates the `Algebraic Normal Form (ANF)` of Grain-128AEAD cipher and determine the linear terms in the equations by differentiating the equations with respect to LFSR and NFSR registers 
  
2. `Verification of attack (Table 2)`
    * This code verifies whether the injected fault at one keystream manages to recover the corresponding register.

3. `Numerically_Find_Fault_locations_S_for_unknowns_in_LFSR`
    * Numerically verify fault injections at S[i] to recovr unknowns in LFSR.
    * If any unknowns can be recovered then the output will indicate the corresponding keystream indices, target register, and recovered unknown.

4. `Verification_recovery_remaining_bits_in_B_using_Grobner_basis`
    * This code solves the equations generated to recover the remaining bits.
  
5. `Obtaining Output Indices where the Output Differential = 1`
    * This code simulates the Grain-128AEAD cipher and compute the output differential and obtains the list of output indices where the results = 1
    
6. `Getting Unique Output Indices for 16 LFSR Bytes`
    * This code gets the output indices of each byte of registers and obtain the unique output indices (remove duplicated)
    
7. `Get Number of Times of Output Differential = 1 for each Output Indices of Each LFSR Byte`
    * This code obtains the number of times of output differential = 1 for single bit of output index for each LFSR Byte
    
8. `Get Number of Times for Output Differential = 1 for Pairs of Output Indices of Each LFSR Byte`
    * This code obtains the number of times of output differential = 1 for pairs of output index for each LFSR Byte

9. `Eq_list_diff_*` <span style="color: grey;">applies to files with this header</span>
    * These codes verifies the results in Table 5 in the paper. The results can be found in `results` folder.

10. `Average no. of required faults S_byte (moderate control)`
    * This code calculates the average numbers of faults to recover the registers in each LFSR bytes in moderate control

### Results
The results and excel files are stored in `results` folder. The folder consists of a couple of `vb` files that are used to highlight the data obtained for better visualisation of the data.