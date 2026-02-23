## Experiment No: 3
DIFFERENTIATOR USING OP-AMP (μA741)
## Aim
To design and simulate a Differentiator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the rate of change of input voltage.
## Apparatus Required
•	μA741 Op-Amp
•	Capacitor C = 0.01 µF
•	Resistor Rf = 10 kΩ
•	Signal Generator
•	Dual Power Supply (±15V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram

<img width="1726" height="972" alt="Screenshot 2026-01-27 140546" src="https://github.com/user-attachments/assets/dd2240da-90e5-41c0-9d2b-7082def697ed" />

## Connection Details:
•	Input signal → Capacitor (C) → Inverting terminal (Pin 2)
•	Feedback resistor (Rf) → Between Output (Pin 6) and Pin 2
•	Non-inverting terminal (Pin 3) → Ground
•	Pin 7 → +15V
•	Pin 4 → −15V
## Theory
A Differentiator circuit produces an output voltage proportional to the rate of change of input voltage.
## Working Principle:
•	When input changes rapidly → output amplitude increases
•	When input is constant → output is zero
•	Output is inverted
## Procedure
1.	Open Proteus software.
2.	Select μA741, capacitor, resistor, signal generator, and CRO.
3.	Connect circuit in differentiator configuration.
4.	Apply ±15V power supply.
5.	Set input sine wave (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.
## Tabulation
| S.No | Input Signal | Frequency (Hz) | Expected Output                  | Practical Observation             |
| ---- | ------------ | -------------- | -------------------------------- | --------------------------------- |
| 1    | Sine (2V)    | 100            | Large amplitude, 90° phase shift | High amplitude, slight distortion |
| 2    | Sine (2V)    | 200            | Reduced amplitude                | Slightly lower output             |
| 3    | Sine (2V)    | 500            | Further reduced amplitude        | Clearly reduced output            |
| 4    | Sine (2V)    | 1k             | Small amplitude                  | Small output waveform             |
| 5    | Sine (2V)    | 2k             | Very small output                | Very low amplitude                |

## Waveforms
•	Sine input → Cosine output (90° phase shift)
•	Square input → Positive & negative spikes
•	Triangular input → Square wave

<img width="1373" height="875" alt="Screenshot 2026-01-27 140525" src="https://github.com/user-attachments/assets/d075232e-c0a5-4bb3-9916-9a76fbb42bd8" />

## Result
The Differentiator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the rate of change of input voltage.
The circuit behaves as a differentiator.
## Conclusion
•	Output depends on frequency.
•	Output leads input by 90° (for sine input).
•	Higher frequency → Higher output amplitude.
•	Used in wave shaping and signal processing applications.
## Viva Questions
1.	What is a differentiator?
2.	Write the output equation of differentiator.
3.	Why is output leading input?
4.	What happens at very high frequency?
5.	What is practical differentiator?
## Answers
1.  A differentiator is an op-amp circuit that produces an output voltage proportional to the rate of change of the input voltage.<br>
2.  Vout = -RC(dVin/dt)<br>
3.  Because differentiation of a sine wave produces a cosine wave, resulting in a 90° phase lead. Hence, output leads input.<br>
4.  At very high frequency, gain increases and the circuit amplifies noise, causing instability.<br>
5.  A practical differentiator includes additional resistor and capacitor components to limit high-frequency gain and improve stability.<br>

