# spiderbob

**spiderbob is a project combining robotics and artificial intelligence.**

---

## Table of Contents / Sommaire

- [Goal of spiderbob](#goal-of-spiderbob)
- [Logbook](#logbook)

---

## Goal of spiderbob

- The main objective of spiderbob is to improve my skills in mobile robotics and AI following the [DeepSight-Nebula](https://github.com/TheValll/DeepSight-Nebula) project.

---

## Logbook

In this section, I'll document my project, take notes, post results, and reflect on my work.

### 11/13/2026

I started by assessing the project's feasibility and budget. My current plan is an autonomous hexapod with three degrees of freedom per leg, 18 servomotors, a 3D camera, and a 360° LiDAR.

I found a used [Intel RealSense D435i](https://www.realsenseai.com/products/depth-camera-d435i/) on Leboncoin for €200, compared with an observed new price of €538.80.

#### LiDAR comparison

I compared multiple lidar; for my usage, the SLAMTEC RPLIDAR C1 has the best compromise.

| Manufacturer | Model       | Advertised maximum range | Price considered | Notes                                                                 | Official link                                                                        |
| ------------ | ----------- | ------------------------ | ---------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| SLAMTEC      | RPLIDAR C1  | 12 m                     | €83.90           | IP54, ToF technology, documentation and ROS 2 driver                  | [RPLIDAR C1 specifications](https://www.slamtec.com/en/c1/spec)                      |
| YDLIDAR      | T-mini Plus | 12 m                     | ~€68–90          | Very compact; advertised resistance to ambient light up to 60,000 lux | [T-mini Plus](https://www.ydlidar.com/product/category/tof/ydlidar-t-mini-plus.html) |
| LDROBOT      | D500        | 12 m                     | ~€60–79          | Compact; 5,000 measurements/s; ROS/ROS 2 support                      | [LDROBOT sensors](https://www.ldrobot.com/sensors)                                   |

#### Servomotor comparison

Same for the servomotor, the dynamixel XL430-W250-T gets the best comparison and feedback on reddit and more stuff, I also found an offer on Leboncoin for 18 servomotors without cables at €320. So I'll buy them.

| Manufacturer | Model                  | Advertised stall torque | Price considered  | Notes                                                                | Link                                                                                   |
| ------------ | ---------------------- | ----------------------- | ----------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| ROBOTIS      | Dynamixel XL430-W250-T | 1.5 N·m                 | €17.78 each, used | Official SDK, ROS 2 support; used on the Hexapod Make 2              | [ROBOTIS XL430-W250-T](https://en.robotis.com/shop_en/item.php?it_id=902-0135-000)     |
| Feetech      | STS3215-C018 (12 V)    | ~2.94 N·m               | €23.90 each, new  | Metal gears, encoder; used in LeRobot projects and personal hexapods | [GoTronic STS3215-C018](https://www.gotronic.fr/art-servo-serie-360-deg-12v-48041.htm) |
| Hiwonder     | HX-35H                 | ~3.43 N·m               | $18.99 each, new  | Used on the JetHexa; high advertised torque                          | [Hiwonder HX-35H](https://www.hiwonder.com/products/hx-35h)                            |
