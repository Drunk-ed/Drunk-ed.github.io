<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Coordinated Bimanual Teleoperation via Haptic Device</title>

  <style>
    h2 {
      margin-bottom: 4px;
    }

    p {
      margin-top: 4px;
      line-height: 1.6;
    }

    h3 {
      margin-top: 20px;
    }

    hr {
      margin: 30px 0;
    }
  </style>
</head>

<body>

  <img src="/images/image.png" alt="Project Image" style="max-width:100%; height:auto;"/>

  <h2 style="color:red;">Project Overview</h2>
  <p>
    <strong>Phantom_to_Interbotix_teleop</strong> is a ROS&nbsp;2–based teleoperation framework that enables real-time,
    intuitive control of an <strong>Interbotix RX200 robotic arm</strong> using a
    <strong>Geomagic Touch (Phantom) haptic device</strong>. The project bridges human hand motions captured by a
    force-feedback stylus with precise robotic arm movements, allowing an operator to manipulate the robot’s
    end-effector in a natural and responsive manner.
  </p>

  <p>
    This system is particularly useful in robotics research, prototyping, and educational environments where
    human-in-the-loop control and intuitive manipulation are required.
  </p>

  <hr>

  <h2>Motivation and Objectives</h2>
  <p>
    Robotic manipulation often requires fine-grained, intuitive control that can be difficult to achieve using
    traditional interfaces such as keyboards or joysticks. The main objectives of this project are:
  </p>

  <ul>
    <li>To provide a <strong>natural teleoperation interface</strong> for controlling a robotic arm</li>
    <li>To integrate <strong>haptic input devices</strong> with ROS&nbsp;2-based robotic systems</li>
    <li>To enable <strong>real-time end-effector and gripper control</strong></li>
    <li>To serve as a flexible base for future extensions in teleoperation and haptics research</li>
  </ul>

  <hr>

  <h2>System Architecture</h2>
  <p>
    The system follows a publisher–subscriber architecture using ROS&nbsp;2:
  </p>

  <ul>
    <li>The <strong>Geomagic Touch device</strong> publishes pose, orientation, and button state data</li>
    <li>The <strong>teleoperation node</strong> subscribes to these topics</li>
    <li>Input data is mapped to motion commands for the <strong>Interbotix RX200</strong></li>
    <li>Commands are sent to the robot using Interbotix ROS&nbsp;2 control interfaces</li>
  </ul>

  <p>
    The teleoperation loop runs at approximately <strong>50&nbsp;Hz</strong> to ensure stable and smooth robot motion.
  </p>

  <hr>

  <h2>Key Features</h2>

  <h3>Real-Time Teleoperation</h3>
  <ul>
    <li>Continuous mapping of stylus position to robot end-effector motion</li>
    <li>Low-latency response suitable for manipulation tasks</li>
  </ul>

  <h3>Multi-Mode Control</h3>
  <ul>
    <li><strong>Cartesian control</strong> for end-effector movement</li>
    <li><strong>Joint-level control</strong> for wrist rotation</li>
    <li><strong>Button-based mode switching</strong> using the Phantom stylus</li>
  </ul>

  <h3>Gripper Control</h3>
  <ul>
    <li>Simple toggle-based gripper open/close functionality</li>
    <li>Integrated with Interbotix gripper APIs</li>
  </ul>

</body>
</html>
