title: Smart Snacks
description: Vending made easy and accesible! 

## Final Project Report

## Final Product Video

https://drive.google.com/file/d/1lTHKj5yUkoilbuedlj4VtLLLDRASPVqX/view?usp=sharing
https://drive.google.com/file/d/1oSQscpiDDHZ8qvP-j2nmh_2r2TbfWnoP/view?usp=sharing


## Final Product Images

![WhatsApp Image 2025-04-26 at 01 06 25](https://github.com/user-attachments/assets/9e2b2134-352b-40c7-85a2-186c6b5f2317)

![WhatsApp Image 2025-04-26 at 01 06 25 (3)](https://github.com/user-attachments/assets/cf4b4d40-9edf-4173-b8e2-2c7cd1b34121)

![WhatsApp Image 2025-04-26 at 01 06 25 (2)](https://github.com/user-attachments/assets/98362f35-b4a3-4773-a42a-8e97ff494d54)

![WhatsApp Image 2025-04-26 at 01 06 25 (1)](https://github.com/user-attachments/assets/d3ec1e72-68dd-46a5-93d7-3991deb04592)

<img width="1464" alt="Screenshot 2025-04-26 at 11 21 22 PM" src="https://github.com/user-attachments/assets/c6038575-a46e-4ae2-9c1d-54d57875d4f6" />

<img width="834" alt="Screenshot 2025-04-26 at 11 21 08 PM" src="https://github.com/user-attachments/assets/6dc424a0-e471-4406-ae5e-6ec80e1fdcc1" />

## Two Topics:
- Timers: Fast PWM for Motor Dispensing
- Power Management: 10V Supply for Motors and 5V for ATMega
- ADC: Ultrasonics for coin and snack detection and keypad

## Input Device:
- Ultrasonic Sensors

## Output Device:  
- LCD Screen

## Serial Communicaiton:  
- LCD over I2C
- UART between 2 ATMegas

## SRS Validation
- **SRS-01**
- The system shall detect user snack selection through a 3-key keypad and store the selection index within 5 seconds of keypress.
  
- **SRS-02**
- Upon coin insertion, the system shall acknowledge the detection within 2 seconds by receiving a UART signal and sending an acknowledgment integer back over UART.

- **SRS-03**
- After snack dispensing is initiated, the system shall detect a dispensed item within 15 cm of the distance sensor and confirm the dispense event within 10 seconds.

- **SRS-04**
- The system shall transmit the selected snack index over UART to the motor controller within 2 seconds of receiving a motor request signal.

- **SRS-05**
- The system shall display updated snack stock and balance information on the LCD screen within 3 seconds after a successful coin insertion and snack selection.

- **Validation Proof:**
![IMG_1674](https://github.com/user-attachments/assets/e4a1d21c-961d-4595-978f-c76e7fb4016d)
<img width="626" alt="Screenshot 2025-04-27 at 9 43 58 PM" src="https://github.com/user-attachments/assets/a4d4515a-b1e3-4f79-affb-f560387c238a" />
![IMG_1672](https://github.com/user-attachments/assets/050a0c91-823d-4c59-8d10-8e8f168efbf7)
  
## HRS Validation
- **HRS-01: Motor Control for Dispensing**  
The motor activates upon when there is sufficient balance detected and spins at the desired PWM speed. It reliably stops within ±3 seconds of a snack being detected by the ultrasonic sensor, preventing double-dispensing.

- **HRS-02: LCD Display Operation**  
- The LCD operates at 5V and displays clear, readable text within ±5% of the expected contrast level. Text updates are consistent and easily visible under normal lighting conditions.

- **HRS-03: Ultrasonic Sensor**
- Detects dropped snacks effectively within a precise range of 5 cm, utilizing advanced UART communication technology to promptly stop the motor from dispensing any additional snacks when a drop is detected. This innovative feature ensures minimal waste and optimal snack management.
Detects quarters as they roll down the ramp with a precise range of 4.5cm.

- **Validation Proof:**
<img width="420" alt="Screenshot 2025-04-27 at 10 13 13 PM" src="https://github.com/user-attachments/assets/e448de86-a38e-4837-9cfb-be6b17b1be93" />
<img width="425" alt="Screenshot 2025-04-27 at 10 12 46 PM" src="https://github.com/user-attachments/assets/a7448f28-bd4c-46ed-af6d-62310423a07d" />
<img width="364" alt="Screenshot 2025-04-27 at 10 12 35 PM" src="https://github.com/user-attachments/assets/6e40f540-93a5-4938-b0ea-d4f249801052" />
<img width="240" alt="Screenshot 2025-04-27 at 10 12 21 PM" src="https://github.com/user-attachments/assets/32341e1f-80a3-4e87-bbdf-82493365e56a" />

## Conclusion
- **What went well and what did you gain from the experience?**
From this experience, we learned that adaptability is key in navigating the complexities of project planning. The necessity to pivot when faced with unexpected challenges pushed us to develop creative solutions and fostered a collaborative spirit among the team. Our collaboration was undoubtedly one of the highlights. Despite encountering tough situations such as encountering an error a few minutes away from the final demonstration, we managed to maintain clear communication and supported one another, ensuring that we solved the issue as soon as possible without losing momentum.

- **What accomplishments are you proud of?**  
We took pride in successfully using UART communication between the 2 Atmega328PBs in order to fully complete the dispensing of snacks without any fault. There were many errors that were unknown to us at the time from loose wires to some tiny mistake in the code , but the fact we broke down every single possible detail in order to figure out what was wrong definitely was one of our main strengths in bringing the machine together. 
Demonstrating a willingness to take a step back in order to reassess and identify areas for improvement in various situations is a notable achievement of which we are proud. Although the decision to revisit our progress may have initially caused feelings of frustration and disappointment, the eventual outcomes validated the effort and proved worthwhile.

- **Did you have to change your approach and did you encounter obstacles that you didn’t anticipate ?**  
We did have to change our approach as we faced difficulties with integrating the IR sensors which were too sensitive. However, we quickly brainstormed and switched to using an Ultrasonic sensor. We also changed our design to fit everything perfectly. We also had to account for the speed of the coin to perform the coin detection mechanism and toggle the motors to find the perfect PWM. 
  
- **What could be a next step for this project?**  
As for next steps,  we should analyze the feedback received on the final product and explore opportunities for enhancements or additional features. This will ensure we continue to innovate and exceed the expectations of our audience. Improved security system by using RFID or contactless payments can further enhance this project as well

---

