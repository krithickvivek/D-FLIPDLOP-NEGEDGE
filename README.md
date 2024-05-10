# D-FLIPDLOP-NEGEDGE

**AIM:**

To implement  D flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**D Flip-Flop**

D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/48c81fe8-bc3f-40e7-95e2-519fc155ad51)

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/e5f3fda7-68ec-4a3a-a0a4-cf6f9cc4ab55)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/8592c0d8-2917-4142-91b9-d6c30dd891d2)

Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

**Procedure**
### Step 1: 
Open Quartus II in your laptop.

### Step 2: 
Write code to implement SR flipflop using verilog and validating their functionality using their functional tables.

### Step 3: 
Run compilation to check for errors.

### Step 4: 
Open waveform output and load input values.

### Step 5: 
Run simulation to get the output.

### Step 6: 
Open in RTL viewers to get RTL diagram output. */

**PROGRAM**

``` 
Program for flipflops and verify its truth table in quartus using Verilog programming.
Developed by: Krithick Vivekananda
RegisterNumber:212223240075
module EXP_8(D,Clock,reset,Q,Qbar);
input D,Clock,reset;
output reg Q,Qbar;
always @(negedge Clock)
if(!reset)
	Q<=0;
else
	Q<=D;
endmodule

```

**RTL LOGIC FOR FLIPFLOPS**
![322782970-35809b70-dde5-443c-9a95-10c4dd6bdf68](https://github.com/krithickvivek/D-FLIPDLOP-NEGEDGE/assets/139331296/3eed490d-a932-4990-89f6-a66f36eabac6)



**TIMING DIGRAMS FOR FLIP FLOPS**

![322783107-dff86801-d6d6-4050-a4c5-cf1222b09713](https://github.com/krithickvivek/D-FLIPDLOP-NEGEDGE/assets/139331296/ed90708b-2e15-4791-b3a2-f86a2f29bd8b)


**RESULTS**

Thus,the T flipflop using verilog and validating their functionality using their functional tables was implemented.
