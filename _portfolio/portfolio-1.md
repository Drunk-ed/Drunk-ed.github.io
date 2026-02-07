---
title: "Coordinated Bimanual Teleoperation via Haptic Device"
excerpt: "Built a real-time bimanual control system in ROS 2 where a secondary ReactorX-200 robot arm mirrors the movements of a teleoperated leader arm."
collection: portfolio
---
<br/><img src='/images/image.png'>
## Project Overview
**Phantom_to_Interbotix_teleop** is a ROS 2–based teleoperation framework that enables real-time, intuitive control of an **Interbotix RX200 robotic arm** using a **Geomagic Touch (Phantom) haptic device**. The project bridges human hand motions captured by a force-feedback stylus with precise robotic arm movements, allowing an operator to manipulate the robot’s end-effector in a natural and responsive manner.

This system is particularly useful in robotics research, prototyping, and educational environments where human-in-the-loop control and intuitive manipulation are required.

---

## Motivation and Objectives
Robotic manipulation often requires fine-grained, intuitive control that can be difficult to achieve using traditional interfaces such as keyboards or joysticks. The main objectives of this project are:

- To provide a **natural teleoperation interface** for controlling a robotic arm
- To integrate **haptic input devices** with ROS 2-based robotic systems
- To enable **real-time end-effector and gripper control**
- To serve as a flexible base for future extensions in teleoperation and haptics research

---

## System Architecture
The system follows a publisher–subscriber architecture using ROS 2:

- The **Geomagic Touch device** publishes pose, orientation, and button state data
- The **teleoperation node** subscribes to these topics
- Input data is mapped to motion commands for the **Interbotix RX200**
- Commands are sent to the robot using Interbotix ROS 2 control interfaces

The teleoperation loop runs at approximately **50 Hz** to ensure stable and smooth robot motion.

---
## Key Features
### Real-Time Teleoperation
- Continuous mapping of stylus position to robot end-effector motion
- Low-latency response suitable for manipulation tasks

### Multi-Mode Control
- **Cartesian control** for end-effector movement
- **Joint-level control** for wrist rotation
- **Button-based mode switching** using the Phantom stylus

### Gripper Control
- Simple toggle-based gripper open/close functionality
- Integrated with Interbotix gripper APIs

---

## Repository Structure

