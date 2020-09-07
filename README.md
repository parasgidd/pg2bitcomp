## 1. Implementation of Power Gating technique in comparator for Low-power applications.
Implementation of Power Gating technique in comparator for Low-power applications.
This repository contains simulation files and other relevant files of project **Implementation of Power Gating technique in comparator for Low-power applications.**
In this project I've implemenbted Power Gating technique for 2 bit Comparator & Studied different aspects of power reduction techniques in low-power VLSI design.



## Table of Contents
- [1. Power Gating technique in comparator for Low-power applications.](#1.-Implementation-of-Power-Gating-technique-in-comparator-for-Low-power-applications.)
- [2. Theory](#2-Theory)
- [3. EDA Tools Used](#4-eda-tools-used)
- [4. Pre-layout Simulations](#5-Pre-layout-Simulations)
- [5. Post-layout and Simulations](#6-Post-Layout-Simulations)
- [6. Future work](#7-Future-work)
- [7. Author](#8-Author)
- [8. Contributors](#9-Contributors)
- [9. Acknowledgments](#10-acknowledgments)
- [10. Contact Information -](#10-contact-information--)

## 2. Theory
 
Comparator is one of the basic fundamental block used in electronics. As the name suggests comparator compares 2 of its inputs & gnerate results at the output end. 
the type of comparator i've used in my project is 'digital comparator', which compare 2 binary bits & generate result (Smaller, Equal & Greater).

</p>

![Alt Text](https://github.com/parasgidd/pg2bitcomp/blob/master/images/general1bitbd.png)

</p>

Fig: 1 - bit Digital Comparator.
</p>

In similar manner, for n-bit comparison --> N blocks of 1-bit comparators are used in pararllel.
but as we know, MSB decides if its smaller or greater, there is no need of computation for further bits once we know if MSB comparison result is smaller or greater. only when M.S.B. comparison generates equal result, we have to look after further bits.

</p>

As we can decide only by MSB comparison & there is no need of comparison of other bits (when MSB are Different), we can completely cutoff power of other parallel connected comparators, without affecting output result. for better understanding its explained in block diagram shown below

</p>

![Alt Text](https://github.com/parasgidd/pg2bitcomp/blob/master/images/generalbd.png)

</p>
Fig: Block Diagram representing general idea of implementation of power gating in n-bit comparator


