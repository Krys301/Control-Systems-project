# ⚙️ Ball and Beam Balancing System (PID Control)

<p align="center">
  <a href="https://github.com/Krys301/Control-Systems-project/blob/main/EE191-Group2%20Technical%20Report%20(Final)%20(2).pdf">
    <img src="https://img.shields.io/badge/📄_View_Technical_Report-blue?style=for-the-badge" alt="Technical Report"/>
  </a>
  <a href="https://github.com/Krys301/Control-Systems-project/blob/main/EE191%20Balance%20Beam%20Project%20Presentation%202025-10-22.pdf">
    <img src="https://img.shields.io/badge/🖥️_View_Presentation-green?style=for-the-badge" alt="Presentation Slides"/>
  </a>
</p>

This project demonstrates a **Ball and Beam Control System** using a **PID controller** to balance a ball at a desired position along a beam.  
The system uses an **ultrasonic sensor** to detect position and a **stepper motor** to adjust the beam angle in real time.

---

## 🎯 Objective
The goal of this project is to maintain the ball at the **setpoint position (≈22 cm)** by dynamically tilting the beam using feedback from the ultrasonic sensor.  
A **PID controller** continuously corrects the position error by adjusting the motor angle between **90° and 180°**.

---

## 🔩 Hardware Used
- **Arduino MegaPi (Makeblock Ultimate 2.0 Kit)**
- **Ultrasonic Sensor (PORT_6)**  
- **28BYJ-48 Stepper Motor** driven via **ULN2003**
- **Custom 44 cm Beam**
- **3D-printed Mounts and Support Frame (optional)**

---

## 🧮 Software & Control
- **PID Controller** implementation in Arduino code  
  - `P` (Proportional): adjusts based on position error  
  - `I` (Integral): compensates steady-state error  
  - `D` (Derivative): smooths the response and reduces overshoot  
- Real-time feedback from the ultrasonic sensor  
- Mapping of distance (0 – 30 cm) to beam angle (90 – 180°)

---

## 📊 Results
- Ball stabilizes within ±1 cm of setpoint after fine PID tuning  
- Demonstrates feedback control principles taught in **EE114 Systems And Controls**  
- Visual indicator via serial monitor or LED feedback  

---

## 🚀 Future Improvements
- Integrate data logging to plot sensor feedback over time  
- Add an LCD display to show ball position and PID output  
- Implement adaptive or fuzzy PID tuning  
- Simulate system dynamics in MATLAB/Simulink for comparison  

---

## 🧑‍💻 Author
**Krystian Stratynski**  
Aspiring AI Prompt Engineer & Software Developer  
[LinkedIn](https://www.linkedin.com/in/krystian-stratynski-9613a1336/) · [GitHub](https://github.com/Krys301)
