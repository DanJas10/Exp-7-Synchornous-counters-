# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
/* write all the steps invloved */



### PROGRAM 
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.

Developed by: Dan Jas J

RegisterNumber:  23012930

*/


# CODE:

## up counter:

![Code](https://github.com/DanJas10/Exp-7-Synchornous-counters-/assets/150931233/ef197976-0fc2-42b7-8e28-2c884aae2a32)



## down counter:

![code](https://github.com/DanJas10/Exp-7-Synchornous-counters-/assets/150931233/ae12f9c7-a884-41b7-8509-ba9e1a9e2c62)








# RTL diagram:

## up counter:

![RTL](https://github.com/DanJas10/Exp-7-Synchornous-counters-/assets/150931233/8517d66f-6bd7-4024-a380-d4b79110cca4)




## down counter:

![RTL](https://github.com/DanJas10/Exp-7-Synchornous-counters-/assets/150931233/2c1a0f2c-5d1b-4177-bbee-9299a84e6249)






# TIMING DIGRAMS:

## up count:

![Output](https://github.com/DanJas10/Exp-7-Synchornous-counters-/assets/150931233/d1f7da7c-2842-4879-b722-f9d72740c46f)



## down count:

![timing diagram](https://github.com/DanJas10/Exp-7-Synchornous-counters-/assets/150931233/1a411fd0-11aa-4d70-9571-c208f2522069)







# TRUTH TABLE :

## up count:

![truth table](https://github.com/DanJas10/Exp-7-Synchornous-counters-/assets/150931233/ff0f1777-00ad-455a-b02d-f90421805063)



## down count:

![trut table](https://github.com/DanJas10/Exp-7-Synchornous-counters-/assets/150931233/f0a6d338-f0a1-4eae-8598-a82fd4d31ed1)




# RESULT:

Thus, the up counter and down counter are designed and the truth tables are verified using quartus software.
