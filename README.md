### SYNCHRONOUS-UP-COUNTER
### Date:05-12-2024
#### NAME:SENTHIL ARUNACHALAM .P
#### REG NO:24900904
**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

1.Type the program in Quartus software.
2.Compile and run the program.
3.Generate the RTL schematic and save the logic diagram.
4.Create nodes for inputs and outputs to generate the timing diagram.
5.For different input combinations generate the timing diagram.

**PROGRAM**
![program](https://github.com/user-attachments/assets/b35fda09-857a-4308-ac25-4b452ca6ac69)


**RTL LOGIC UP COUNTER**

![gate](https://github.com/user-attachments/assets/3fc3accb-bbb7-4740-a274-0d0e11d163aa)

**TIMING DIAGRAM FOR IP COUNTER**

![Timing diagram](https://github.com/user-attachments/assets/0ef58726-6104-4f02-ae02-dcf6da80340c)

**TRUTH TABLE**

![Truth Table](https://github.com/user-attachments/assets/a3323548-6efe-46eb-bc7c-21ac97cdf853)

**RESULTS**

Thus the given 4 bit synchronous up counter are implimented using and validate functionality are verified using verilog programming.
