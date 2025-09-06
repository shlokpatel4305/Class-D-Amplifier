# Class-D-Amplifier
This is a schematic for a class-AB audio amplifier circuit. It's designed to take a low-level audio input and amplify it to drive a speaker. The circuit operates from a single 12V DC power supply.

Key Components and Stages
Input Stage (Q1): The audio signal enters through the "Audio In" jack (J2) and is coupled to the base of a Q1 transistor. This is a common emitter amplifier stage that provides voltage gain.

Voltage Amplifier Stage (LM383): The amplified signal from Q1 is fed into an LM383 audio power amplifier IC. This IC is the heart of the circuit, providing significant voltage gain and driving the output stage. The resistors and capacitors around the IC are for setting the gain and ensuring stability.

Class-AB Push-Pull Output Stage (Q3, Q4): The output from the LM383 IC drives a complementary pair of power transistors, Q3 and Q4. This is a class-AB configuration, which minimizes crossover distortion—a common issue in class-B amplifiers—by ensuring both transistors are slightly "on" even at zero signal. Q3 is an NPN transistor (e.g., 2N3904), and Q4 is a PNP transistor (e.g., 2N3906). This push-pull arrangement allows the circuit to efficiently drive current into the speaker during both the positive and negative cycles of the audio waveform.

Output Filter (L1, C7): The output of the push-pull stage is passed through an LC filter (L1 and C7). This filter is crucial for smoothing the signal and removing any high-frequency switching noise before the signal reaches the speaker.

Speaker Output (J3): The final amplified audio signal is delivered to the speaker through the "Speaker" jack (J3).

Power and Indicator: The circuit is powered by a 12V DC source through the power jack (J1). LED1 serves as a power indicator, lighting up when the circuit is on.

This circuit provides a good balance of power efficiency and audio fidelity, making it suitable for a variety of audio projects.
