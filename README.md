
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

Fiber optic links can be used for transmission of digital as well as analog signals. Basically a fiber optic link contains three main elements, a transmitter, an optical fiber and a receiver. The transmitter module takes the input signal in electrical form and then transforms it into optical (light) energy containing the same information. The optical fiber is the medium which takes the energy to the receiver. At the receiver light is converted back into electrical form with the same pattern as originally fed to the transmitter.

TRANSMITTER:
Fiber Optic transmitters are typically composed of a buffer, driver and Optical Source. The buffer electronics provides both an electrical connection and isolation between the transmitter and the electrical system supplying the data. The driver electronics provides electrical power to the Optical source in a fashion that duplicates the pattern of data being fed to the transmitter. Finally the optical source (LED) converts the electrical current to light energy with the same pattern. The LED SFH450V (950nm) supplied with this kit operates outside the visible light spectrum. Its Optical output is centered at near infrared wavelength of 950nm. The LED SFH756V (660nm) supplied with this kit operates at the visible light spectrum. Its Optical output is centered at wavelength of 660nm.

RECEIVER:
The function of the receiver is to convert the optical energy into electrical form, which is then conditioned to reproduce the transmitted electrical signal in it's original form. The detector SFH350V (Photo Transistor Detector) used in the kit has a transistor type output. The parameters usually considered in the case of detector are it's responsivity at peak wavelength and response time. SFH350V (Photo Transistor Detector) has responsivity of about 0.8mA/10uW at 660nm. But its response time is quite large and thus has lower bandwidth of about 300 KHz. When optical signal falls on the base of the transistor detector, proportional
 
current flows through its emitter generating the voltage across the resistance connected between emitter and ground. This voltage is the duplication of the transmitted electrical signal, which can be amplified.


## PROCEDURE

	Refer to the block diagram & carry out the following connections and settings.
	Connect the power supply with proper polarity to the kit link-B and switch it on.
	Keep all Switch Faults in OFF position.
	Keep switch SW8 towards TX position.
	Keep switch SW9 towards TX1 position.
	Keep Jumper JP5 towards +12V position.
	Keep Jumpers JP6, JP9, JP10 shorted.
	Keep Jumper JP8 towards sine position.
	Keep Intensity control pot P2 towards minimum position.
	Feed about 2Vpp sinusoidal signal of 1 KHz from the function generator to the IN post of Analog Buffer.
<img width="685" height="292" alt="image" src="https://github.com/user-attachments/assets/be05770a-5c8f-4903-a660-6e75e720f63c" />

 
	Connect the output post OUT of Analog Buffer to the post TX IN of Transmitter.
	Slightly unscrew the cap of SFH756V (660nm). Do not remove the cap from the connector. Once the cap is loosened, insert the one meter fiber into the cap. Now tighten the cap by screwing it back.
	Connect the other end of the Fiber to detector SFH350V (Photo Transistor Detector) very carefully.
	Observe the detected signal at post ANALOG OUT on oscilloscope. Adjust Intensity control pot P2 Optical Power control potentiometer so that you receive signal of 2Vpp amplitude.
<img width="743" height="301" alt="image" src="https://github.com/user-attachments/assets/af40437e-8553-47ad-b810-4cc326df05a4" />

	To measure the analog bandwidths of the phototransistor vary the input signal frequency and observe the detected signal at various frequencies.
	Plot the detected signal against applied signal frequency and from the plot determine the 3dB down frequency.
	Keep switch SW9 towards TX2 position.
	Keep Jumper JP7 towards +12V position.
	Remove fiber cable from SFH756V (660nm) and slightly unscrew the cap of SFH450V (950nm). Do not remove the cap from the connector. Once the cap is loosened, insert the one meter fiber into the cap. Now tighten the cap by screwing it back.
	Observe the detected signal at post ANALOG OUT on oscilloscope.

<img width="721" height="292" alt="image" src="https://github.com/user-attachments/assets/99dad300-11e9-452f-80a4-681435feb2b7" />


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
