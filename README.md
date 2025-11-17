
# Exp 4 Experimental verification of frequency response of Analog fiber optic link
# Fiber Optic Link Analysis (660nm)

## AIM
To analyze the relationship between input and received signal of a 660nm fiber optic cable using analog and digital link.

---

## EQUIPMENTS REQUIRED
- Fiber optic trainer kit ST 2502  
- Power supply  
- Patch cords  
- CRO (Cathode Ray Oscilloscope)  
- 660 nm fiber cable  

---

## THEORY

Fiber optic links can be used for transmission of digital as well as analog signals. A fiber optic link typically consists of three main elements:
- **Transmitter**: Converts the electrical input signal into optical (light) energy.
- **Optical Fiber**: Serves as the transmission medium for the light signal.
- **Receiver**: Converts the received light back into an electrical signal, preserving the original signal pattern.

---

## PROCEDURE

1. Connect the power supply to the board.  
2. Ensure that all switched faults are set to ‘Off’.  
3. Make the following connections (as shown in Figure 19):  
   a. Connect the 1KHz sine wave output to emitter 1's input.  
   b. Connect the fiber optic cable between emitter output and detector input.  
   c. Connect detector 1's output to AC amplifier 1 input.  
4. On the board, switch emitter 1's driver to analog mode.  
5. Switch on the power.  
6. Observe the input to emitter 1 (TP5) and the output from AC amplifier 1 (TP28). Verify that both signals are identical.  
7. Vary the frequency between 10 Hz to 1 MHz and observe the output voltage for a constant input voltage of 5V.  
8. Calculate the bandwidth by determining the gain in decibels (dB).  

---

## BLOCK DIAGRAM

<img width="1189" height="704" alt="Screenshot 2025-11-11 190114" src="https://github.com/user-attachments/assets/08881b61-42f8-4e62-95b9-13ff3e4be597" />


---


## TABULATION  
**Transmission through Analog Link**

| Frequency (Hz) | Output Signal Amplitude (Vo) | Gain = Vo/Vi | Gain in dB |
| -------------- | ---------------------------- | ------------ | ---------- |
| 100            | 8.3 V                        | 1.66         | 3.3        |
| 500            | 9.6 V                        | 1.9          | 5.57       |
| 1k             | 10.3 V                       | 2.06         | 6.27       |
| 3k             | 12.2 V                       | 2.44         | 7.74       |
| 5k             | 12.8 V                       | 2.56         | 8.16       |
| 10k            | 12.8 V                       | 2.56         | 8.16       |
| 20k            | 12.8 V                       | 2.56         | 8.16       |
| 50k            | 12.8 V                       | 2.56         | 8.16       |
| 100k           | 12.8 V                       | 2.56         | 8.16       |
| 500k           | 12.8 V                       | 2.56         | 8.16       |
| 1M             | 12.2 V                       | 2.44         | 7.74       |
| 3M             | 9.4 V                        | 1.88         | 5.48       |
| 5M             | 8.3 V                        | 1.38         | 3.97       |

---

## MODEL GRAPH

<img width="880" height="538" alt="Screenshot 2025-11-11 190804" src="https://github.com/user-attachments/assets/25ece563-cf37-448d-8b86-19078ca43f90" />


## GRAPH

![WhatsApp Image 2025-11-17 at 10 52 03_152ebde5](https://github.com/user-attachments/assets/a24e6459-ed7b-4887-b77f-086ebd0faf19)


---

## RESULT

Thus, the frequency response of analog fiber optic link was studied and the determined bandwidth is 95 kHz.
