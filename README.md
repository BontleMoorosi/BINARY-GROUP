# BINARY-GROUP
# **BINARY ADDER  ASSIGNMENT**
## CS3520  COMPUTER ORGANISATION AND ARCHITECTURE
## GROUP MEMBERS
### MOOROSI BONTLE 202201087
### MOLAHLEHI TS'OLO 202202131
### KHANYAPA TLALI 202201987
### MAKHAHLELA KANANELO 202201985
### MPAHANE MOTLATSI 202201288
### JASE BOITUMELO 202201099
### SEKALAKA BAKOENA 202200993



## **OBJECTIVE**
The objective of this project is to design and simulate a 2-bit binary adder using basic digital logic gates like AND, OR, and XOR. The circuit will add two 2-bit binary numbers and output the correct sum and carry. Using simulation, the circuit verifies its functionality and accuracy  of the logic circuit.  Documentation of the entire process, from design to testing , to all errors encountered and over come. The project ensures understanding of  digital logic design and teaches presentation of projeccts using modern collaboration and publishing tools.

## **OUTLINE**

- Design
- Simulation 
- Testing

## **DESIGN**
### Concepts

1.Binary Numbers: Binary is a base-2 number system that uses only two digits: 0 and 1. In binary addition, similar to decimal addition, two numbers are added bit by bit, and if the sum exceeds the largest value in a bit (which is 1), a carry is generated to the next higher bit position.

2. Half Adder: A basic digital circuit that adds two single-bit binary numbers (A and B). It outputs a sum (S) and a carry (C). The sum is calculated using XOR, and the carry is calculated using AND.

   
3. Full Adder: Combines two Half Adders to handle the addition of two bits plus a carry bit. This is required for the most significant bit (MSB).

Full Adder Truth Table
A|B|Cin|Sum(S)|Cout
--|--|--|--|--
0|0|0|0|0
0|0|1|1|0
0|1|0|1|0
0|1|1|0|1
1|0|0|1|0
1|0|1|0|1
1|1|0|0|1
1|1|1|1|1

### Circuit design
#### First Half Adder:
 A basic digital circuit that adds two single-bit binary numbers (A and B). It outputs a sum (S) and a carry (C). The sum is calculated using XOR, and the carry is calculated using AND.
#### Second Half Adder:
Combines two Half Adders to handle the addition of two bits plus a carry bit. This is required for the most significant bit (MSB).
#### OR Gate:
Combine the carry outputs from the two half adders (C0 and C1) to produce the final carry-out (C2).

### Steps in the Circuit

Step 1 (Least Significant Bit Addition)

-Use a half adder to add A0 and B0. 
-This produces the least significant bit of the sum (S0) and a carry-out (C0).

Step 2 (Most Significant Bit Addition)

-Use another half adder to add A1 and B1, along with the carry-out from the first half adder (C0).                                 
-This produces the most significant bit of the sum (S1) and another carry-out (C1).

Step 3 (Final Carry-Out)

-Use an OR gate to combine the carry-outs from the two half adders (C0 and C1) to produce the final carry-out (C2).

### Execution
### TEST 1 (FAULTY IMPLIMENTATION)

First design includes three XOR gates , one AND gate and one OR gate. 
The truth tables of all logic operations where tabled out as to make calculations easier and accurate.
The execution of the  first design proved to be functionally correct when adding the two bit binary numbers (11+11) and gave the correct output of (110). 
Further testing with the two bit binary digits(11+10) , the output was incorrect.This was because the answer provided by the logic gate circuit and the arithmetic calculated answers where completely different.
This signified an error in our logic design  resulting in reworking and figuring out the proper connections of the logic gates.

THE LOGIC GATES DIAGRAM
![Image](https://github.com/user-attachments/assets/a6e2e1f8-9022-4798-b2b5-0a3bead27306)

THE TRUTH TABLES AND COMPUTATION
![Image](https://github.com/user-attachments/assets/ceab2cba-a1f6-436c-a56f-442866ff4f08)

THE FIRST DESIGN OVERVIEW
![Image](https://github.com/user-attachments/assets/a9f0af3c-4781-44fc-9c42-d6c1a7965340)

### TEST 2 (PASSED IMPLIMENTATION)

For the second test we included three XOR gates, two AND gates and one OR gate.
The truth tables of all logic operations where tabled out as to make calculations easier and accurate.
The execution of the second design went along with fear but proved to be a lot more effective when comparing the outputs of the logic circuit and the arithmetic computation. The answer was correct when adding (11+11) and gave the correct output of (110). 
Further testing with the two bit binary digits(11+10) ensured that the logic gate circuit functions for different arithmetic computations helped concluded that the second design was functional.
The change in the logic design and gates helped us figure the correct connection of the gates that works for all two bit binary numbers.

THE LOGIC GATES DIAGRAM

![Image](https://github.com/user-attachments/assets/52041b36-c0a1-457b-96d0-3e08c59dba69)

THE TRUTH TABLES AND COMPUTATIONS

![Image](https://github.com/user-attachments/assets/f90f4d58-d748-4c55-9cae-2bc77d0e4844)

THE SECOND DESIGN OVERVIEW

![Image](https://github.com/user-attachments/assets/43fd549b-b29f-4c86-8920-ec2db40a7d0b)


### **SIMULATION**

For this project we tried using Logisim for the simulation but encountered a few problems. The first problem being finding a secure website to download the required application. Once that problem was tackeled down and solved , we used a different system than required(Java script ) that is usually found in Linux systems not Windows.
Above all odds we retreated back to Digital works that we trust, using Digital works we were able to run different tests of the logic designs we created.

This are some of the examples from our simulation. The full details on our youtube channel.
![image](https://github.com/user-attachments/assets/b65a7be8-68fa-4a8c-aade-c1bdc43befd2)
![image](https://github.com/user-attachments/assets/4f6d71c0-c63c-46a9-ba45-bddfafd230ba)

### **TESTING**
We used digital works to test weither our circuit were arithmetically correct or there was an error in our system. A youtube video attatched to the file details the steps in our testing phase and the errors incurred while testing.
https://youtu.be/cHErCBPIGgA

