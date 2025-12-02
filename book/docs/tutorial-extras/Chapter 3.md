# **Chapter 3: Actuators and Motion Control**

---

## **Introduction to Actuators**
Actuators convert electrical energy into mechanical motion, enabling robots to:  
- Move their joints  
- Manipulate objects  

Key considerations when selecting actuators:  
- Power output  
- Weight  
- Speed  
- Precision  
- Cost  

Humanoid robots require **dozens of actuators working in coordination** to achieve fluid, human-like movement.

---

## **Electric Motors in Robotics**
- **Brushless DC motors (BLDC):** Efficient, controllable, high power density  
- **Servo motors:** Provide precise position control for joint articulation  
- **Stepper motors:** Accurate positioning without feedback sensors  

**Example:** A humanoid robot's shoulder joint might use a high-torque BLDC motor with gear reduction to lift heavy objects while maintaining precise control.

---

## **Hydraulic and Pneumatic Systems**
- **Hydraulic actuators:** Use pressurized fluid to generate high force in compact packages  
  - Example: Boston Dynamics' Atlas robot uses hydraulics for explosive movements and heavy lifting  
- **Pneumatic actuators:** Use compressed air, offering compliance and safety for human interaction  

> Note: Hydraulic systems are heavier and more complex than electric alternatives, suitable for specialized high-power applications.

---

## **Gear Systems and Transmission**
- **Gearboxes:** Reduce motor speed while increasing torque  
- **Harmonic drives:** High gear ratios in compact form, minimal backlash, precise control  
- **Belt and pulley systems:** Transmit motion across distances while maintaining flexibility  

Proper transmission design balances **strength, efficiency, and weight constraints**.

---

## **Motion Control Algorithms**
- **PID (Proportional-Integral-Derivative) controllers:** Adjust actuator commands based on position errors  
- **Model predictive control:** Anticipates future states to optimize trajectories  
- **Impedance control:** Adjusts joint stiffness to comply with external forces, essential for safe human collaboration

---

## **Real-World Application: Walking Gait**
A humanoid robot’s walking gait requires **coordinated control of 12+ joint actuators**:  
- **Ankle actuators:** Rapid adjustments based on IMU feedback to prevent tipping  
- **Hip actuators:** Generate forward propulsion  
- **Knee actuators:** Absorb impact forces during foot strikes  

This demonstrates **integrated actuator control** in a real-world scenario.
