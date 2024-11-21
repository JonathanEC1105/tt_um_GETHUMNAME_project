<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

Finonnaci LFSRs

A 16-bit Fibonacci LFRS. The feedback tap numbers shown correspond to a primitive polynomial in the table, so the register cycles through the maximum number of 65535 states excluding the all-zero state. The state shown, 0xACE1 (hexadecimal) will be followed by 0x5670.
Duration: 30 seconds.0:30 
A Fibonacci 31-bit linear feedback shift with taps at positions 28 and 31, giving it a maximum cycle and period at this speed of nearly 6.7 years. The bit positions that affect the next state are called the taps. In the diagram the taps are [16,13,14,11]. The rightmost bit of the LFSR is called the output bit, wich is always also a tap. To obtain the next bit, the taps bits are XOR-ed sequentially, then, all bits are shifted one bit to the right, with the rightmost bit being discarded, and that result of XOR-ing the tap bits fed back into the now vacant leftmost bit. To obtain the pseudoram output stream, read the rightmost bit after each state transition.  

## How to test

Input clock and reset

## External hardware

ADALM2000
