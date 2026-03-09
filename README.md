## Experiment No: 6
MONOSTABLE MULTIVIBRATOR USING 555 TIMER 
## Aim
To design and simulate a Monostable Multivibrator using NE555 in Proteus Design Suite and verify the time duration of the output pulse.
## Apparatus Required
•	NE555 Timer IC
•	Resistor R = 100 kΩ
•	Capacitor C = 10 µF
•	Push Button (Trigger)
•	DC Power Supply (5V or 9V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
Pin Connections:
•	Pin 1 → Ground
•	Pin 2 → Trigger (Connected to push button)
•	Pin 3 → Output
•	Pin 4 → Reset (Connected to Vcc)
•	Pin 5 → Control Voltage (Optional 0.01 µF capacitor to ground)
•	Pin 6 → Threshold
•	Pin 7 → Discharge
•	Pin 8 → Vcc
<img width="1095" height="638" alt="Screenshot 2026-02-23 221945" src="https://github.com/user-attachments/assets/5d4ee3e5-74dc-4563-b3b6-7155e475bbf1" />

## Circuit Connections:
•	Resistor R → Between Vcc and Pin 7
•	Capacitor C → Between Pins 6 & 7 and Ground
•	Trigger → Pin 2
•	Output → Pin 3
## Theory
A Monostable Multivibrator has only one stable state and one quasi-stable state. It produces a single output pulse when triggered externally.
In monostable mode:
•	The circuit remains in stable LOW state.
•	When a negative trigger pulse is applied at Pin 2 (below 1/3 Vcc), the output becomes HIGH.
•	The capacitor starts charging through resistor R.
•	When capacitor voltage reaches 2/3 Vcc, the output returns to LOW state automatically.
Thus, a single pulse is generated for a fixed time duration.
The NE555 operating in monostable mode acts as a one-shot pulse generator. It has one stable state and one quasi-stable state. Normally, the output remains LOW. When a negative trigger pulse is applied to the trigger pin (Pin 2) below 1/3 Vcc, the output becomes HIGH and remains HIGH for a fixed time interval. During this period, the capacitor connected in the circuit charges through the resistor. When the capacitor voltage reaches 2/3 Vcc, the output automatically returns to LOW state. The pulse width of the output is determined by the resistor and capacitor values and is given by the expression T=1.1RCT = 1.1 RCT=1.1RC. Thus, the 555 timer in monostable mode produces a single output pulse for each trigger input and is widely used in timer and delay applications.
## Procedure
1.	Open Proteus software.
2.	Select NE555 timer, resistor, capacitor, push button, and CRO.
3.	Connect circuit in monostable configuration.
4.	Apply 5V supply.
5.	Press trigger button.
6.	Observe output pulse on CRO.
7.	Measure pulse width.
## Tabulation
S.No	        R (kΩ)	          C (µF)	        Theoretical Pulse Width	            Practical Pulse Width
<img width="670" height="308" alt="Screenshot 2026-02-23 222243" src="https://github.com/user-attachments/assets/f87ac6d9-a3d5-4b75-bb17-7d7793a7fe11" />

## Waveform
•	Trigger → Short negative pulse
•	Output → Single positive pulse
•	Capacitor voltage → Exponential charging waveform
<img width="1064" height="873" alt="Screenshot 2026-02-23 222421" src="https://github.com/user-attachments/assets/9fda2779-6e2b-400d-ba05-7b5be49b75a6" />
<img width="1061" height="882" alt="Screenshot 2026-02-23 222451" src="https://github.com/user-attachments/assets/ea869a64-c719-4d68-b8ed-b6b9d47287b0" />


## Result
The Monostable Multivibrator using NE555 Timer IC was successfully designed and simulated in Proteus.
A single output pulse of duration approximately 1.1 seconds was obtained.
The practical value closely matches the theoretical value.
## Conclusion
•	The circuit produces one output pulse for each trigger.
•	Pulse width depends on R and C values.
•	Increasing R or C increases pulse duration.
•	Used in timers, delay circuits, and pulse generation applications.
## Viva Questions
1.	What is a monostable multivibrator?<br>
A circuit with one stable state that produces a single output pulse when triggered.
2.	Write the pulse width formula.<br>
T=1.1RC
3.	What is the stable state of monostable?<br>
Output LOW.
4.	Why is it called “one-shot”?<br>
Because it generates one output pulse for each trigger input.
5.	What happens if capacitor value increases?<br>
Pulse width increases.

