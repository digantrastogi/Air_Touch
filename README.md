# Air_Touch 🙋‍♂️
A touchless switch using simple circuit based on BJT BC-547. Designed and simulated on LTSpice and hardware prototype developed.
## Project Aim 🎯
1. The aim of this project is to design a hardware circuit prototype for a touchless switch without using expensive components like IR sensors.
2. The design process will first be carried out on SPICE simulation softwares and then the final circuit will be tested on a breadboard. 
3. After getting successful results, the final circuit will be soldered on a copper laminated circuit board.
## Project Background 💡
Covid-19 has increased the need for touchless operation. Switches are a frequently touched surface and can lead to spread of the viral disease to many people. Hence it is important to come up with novel circuits which are power efficient, cheap and easy to build that can implement touchless control. 
The inspiration for this circuit was from the darlington pair. A darlington pair is the combination of two transistors that combined provide high current gain. 
Implementing a 3 transistor circuit for very high current gain was done through LTSpice. 
## Circuit Diagram🔌
<div align="center">
<img width="300" alt="Circuit" src="https://user-images.githubusercontent.com/86347098/123809399-3319d580-d90f-11eb-8c84-a0306e89a561.png">
</div>

## Working ⚙️

The hand when brough near the foil pad, creates a potential difference between the two sides of the pad due to electrostatic induction by the small charges present in our body. 
The potential difference is transferred to the base of transistor-1. 
The potential is then amplified serially one by one by the three transistors, becoming enough to light up the LED
The models are as follow:
<div align="center">
<img width="244" alt="Model" src="https://user-images.githubusercontent.com/86347098/123809989-b0dde100-d90f-11eb-9ba3-804b18b6e9d9.png">  <img width="173" alt="PCB" src="https://user-images.githubusercontent.com/86347098/123809973-ad4a5a00-d90f-11eb-9039-0e9ff180db20.png">
</div>

## Simulation🏃
LTSpice sofwatre was used to design the circuit to light up a off the shelf LED. 
<div align="center">
<img width="388" alt="LTspice" src="https://user-images.githubusercontent.com/86347098/123809697-73795380-d90f-11eb-818a-05c1bac7519d.png">
 <br /> LTSpice model circuit
</div> <br />

The results are as follows:  <br />
1. Input current is as follow: <br />
 <br />
<img width="410" alt="InputCurrent" src="https://user-images.githubusercontent.com/86347098/123810765-4aa58e00-d910-11eb-8ea6-3276c4476972.png">
<br />
2. After current amplification by transistor-1  <br />
 <br />
<img width="413" alt="CurrentAfterAmplificatio1" src="https://user-images.githubusercontent.com/86347098/123809792-8855e700-d90f-11eb-8a76-6f34080d57f1.png">
<br />
3. After current amplification by transistor-2  <br />
 <br />
<img width="413" alt="CurrentAfterAmplificatio2" src="https://user-images.githubusercontent.com/86347098/123809877-999ef380-d90f-11eb-8336-8859def815e0.png">
<br />
4. Final current through LED  <br />
  <br />
<img width="413" alt="CurrentAfterAmplificatio3" src="https://user-images.githubusercontent.com/86347098/123809931-a4598880-d90f-11eb-81d8-a7cfedd088cf.png">
 <br />
 
## Conclusion 📌

As can be seen the circuit successfully amplifies a current of 100 nA to 22 mA, sufficient for switching on an LED light. Hence when hand is brotuh near the antenna a very small current will be induced which will be successively to light up the LED.

## Technology Stack 🛠️
- **Coding Languages**: SPICE

- **Tools & Technologies**: LTSpice

- **Project Management Tools**: Trello, Git/Github, Markdown (Documentation), Microsoft powerpoint, LaTeX

## Learning Resources 🧰

-   [Introduction to LTSpice](https://www.analog.com/en/analog-dialogue/articles/get-up-and-running-with-ltspice.html)
    
-   [Darligton Pair](https://en.wikipedia.org/wiki/Darlington_transistor)
    
## License📜
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


