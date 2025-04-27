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


## SRS Validation
- **SRS-01: Coin Detection**  
  Detected via ultrasonic sensor interrupts and verified using UART logs.

- **SRS-02: Coin Value Reading & Balance Update**  
  Updates displayed on LCD within 1 second. UART logs confirm real-time updates.

- **Validation Proof:**  
  Oscilloscope captures and UART screenshots showing system responses.

## HRS Validation
- **HRS-01: Motor Control for Dispensing**  
  Motor spins correctly on product selection and stops on snack detection.

- **HRS-02: Inventory Tracking**  
  Inventory is updated after detecting the dropped product using an ultrasonic sensor.

- **Validation Proof:**  
  Videos and UART debug showing real-time distance detection and item tracking.

## Conclusion
- **What did you learn from it?**  
  Real-world integration of embedded systems and mechanical systems.
  
- **What went well?**  
  Coin detection and inventory tracking were reliable and responsive.

- **What accomplishments are you proud of?**  
  Successful coordination of hardware-software integration.

- **What did you gain from this experience?**  
  Practical skills in microcontroller programming, UART, and circuit design.

- **Did you have to change your approach?**  
  Adjusted coin detection to reduce false triggers caused by mechanical vibration.

- **What could have been done differently?**  
  Earlier mechanical reinforcement to avoid spiral misalignments.

- **Did you encounter obstacles that you didn’t anticipate?**  
  Motor mounting challenges and vibration noise affecting ultrasonic readings.

- **What could be a next step for this project?**  
  Adding RFID authentication for product retrieval and building a multi-row vending structure.

---

✅ GitHub repository updated.  
✅ Final video and documentation completed.  
✅ README meets final project submission guidelines.

