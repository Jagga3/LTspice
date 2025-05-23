# CMOS INVERTER
This repository contains the design, simulation, and analysis of a CMOS Inverter — a fundamental building block in digital electronics. It demonstrates how complementary MOSFETs (PMOS and NMOS) work together to implement digital logic.

## 📌 Project Overview

A CMOS Inverter uses a PMOS transistor connected to VDD and an NMOS transistor connected to GND. When the input is high, the NMOS conducts and pulls the output low; when the input is low, the PMOS conducts and pulls the output high. This configuration offers:

* Low static power consumption

* High noise margins

* Full rail-to-rail output voltage swing

##  Circuit Design 

![Image](https://github.com/user-attachments/assets/f90a65b1-42f2-43e9-8671-9ceeb4f146e0)

## Schematic

![Image](https://github.com/user-attachments/assets/5341e87f-9a29-4c75-bce1-f040aeb6028b)

 
## 🛠️ Step-by-Step: Designing CMOS Inverter 

## Tool : LTspice

1. Launch LTspice

Open LTspice

Choose File > New Schematic

2. Add Components

## 📌 You'll need:

1 × PMOS transistor (pMOS)

1 × NMOS transistor (nMOS)

1 × Vdd (DC voltage source)

1 × Input voltage source (Vin)

1 × Ground

## 📌 How to:

Press F2 or click the component symbol (AND gate icon)

Search or scroll to find:

nmos

pmos

Voltage

## 📌 Build the Inverter Circuit

Connections:

PMOS:

Source → Vdd

Gate → Input (Vin)

Drain → Output node

NMOS:

Source → GND

Gate → Input (Vin)

Drain → Output node

NMOS:

Source → GND

Gate → Input (Vin)

Drain → Output node (shared with PMOS drain)

Connect Vdd (e.g., 5V) between a voltage source and GND

Connect Vin using a PULSE input for transient or DC sweep for DC analysis

## 📌 Set Input Voltage Source

For transient simulation, use:

spice

V1 IN 0 PULSE(0 2 2 0.001 0.001 2 4)

0 → low voltage

2 → High voltage

2 → delay

0.001 → rise/fall time

2 → on time

4 → total period

## 📌 Run Simulations

🧪 DC Sweep:

 Transient:

Click .tran → Enter:

.tran 8

Run the sim, then plot output (V(out)) and input (V(in))

Verify the output by tallying the truth table

## truth table

| Input (A)  |   Output(Y = NOT A)  |
|------------|----------------------|
|   0        |          1           |
|   1        |         	0           |


## Output Waveform

![Image](https://github.com/user-attachments/assets/74067b88-ee44-4d7d-b203-3c764ca6dcce)

Design file `inverter.asy` 

# 🤝 Contributing
Contributions are welcome! Please open an issue or submit a pull request if you’d like to improve this project — whether it’s optimizing the layout, improving simulation scripts, or adding testbenches.

# 📄 License
This project is licensed under the MIT License.

## contact me

LinkedIn : http://www.linkedin.com/in/jagadeesh-bathula-246aba300

Mail : jagadeeshbattula0@gmail.com
