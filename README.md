# jiwanshi.github.io
Final Project Report

## Final Product Video
https://drive.google.com/file/d/1lTHKj5yUkoilbuedlj4VtLLLDRASPVqX/view?usp=sharing
https://drive.google.com/file/d/1oSQscpiDDHZ8qvP-j2nmh_2r2TbfWnoP/view?usp=sharing
- The video shows the vending machine working end-to-end: coin detection, balance updates, motor dispensing, and inventory tracking.  

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
- **SRS-01: Coin Detection**
- The coin is detected using an ultrasonic sensor positioned at the coin slot. An interrupt is triggered within 20 ms of the coin passing the sensor, and a counter is incremented. UART debug logs confirm successful detection and tracking of the number of coins inserted.
  
- **SRS-02: Snack Detection**
- After motor activation, an ultrasonic sensor at the dispensing area detects when a snack has fallen. If an object is detected within a specified distance threshold, the system stops the motor to prevent double dispensing. Detection times were verified through UART logs and oscilloscope captures.

- **Validation Proof:**
![IMG_1674](https://github.com/user-attachments/assets/e4a1d21c-961d-4595-978f-c76e7fb4016d)
<img width="626" alt="Screenshot 2025-04-27 at 9 43 58 PM" src="https://github.com/user-attachments/assets/a4d4515a-b1e3-4f79-affb-f560387c238a" />
![IMG_1672](https://github.com/user-attachments/assets/050a0c91-823d-4c59-8d10-8e8f168efbf7)
  
## HRS Validation
- **HRS-01: Motor Control for Dispensing**  
The motor activates upon when there is sufficient balance detected and spins at the desired PWM speed. It reliably stops within ±3 seconds of a snack being detected by the ultrasonic sensor, preventing double-dispensing.

- **HRS-02: LCD Display Operation**  
- The LCD operates at 5V and displays clear, readable text within ±5% of the expected contrast level. Text updates are consistent and easily visible under normal lighting conditions.

- **Validation Proof:**
<img width="420" alt="Screenshot 2025-04-27 at 10 13 13 PM" src="https://github.com/user-attachments/assets/e448de86-a38e-4837-9cfb-be6b17b1be93" />
<img width="425" alt="Screenshot 2025-04-27 at 10 12 46 PM" src="https://github.com/user-attachments/assets/a7448f28-bd4c-46ed-af6d-62310423a07d" />
<img width="364" alt="Screenshot 2025-04-27 at 10 12 35 PM" src="https://github.com/user-attachments/assets/6e40f540-93a5-4938-b0ea-d4f249801052" />
<img width="240" alt="Screenshot 2025-04-27 at 10 12 21 PM" src="https://github.com/user-attachments/assets/32341e1f-80a3-4e87-bbdf-82493365e56a" />

## Conclusion
- **What did you learn from it?**  
  
  
- **What went well?**  
  

- **What accomplishments are you proud of?**  
 

- **What did you gain from this experience?**  
  

- **Did you have to change your approach?**  
  

- **What could have been done differently?**  
  

- **Did you encounter obstacles that you didn’t anticipate?**  
  

- **What could be a next step for this project?**  
  

---

