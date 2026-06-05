---
layout: page
title: Autonomous Agricultural Robot
description: A ground robot for autonomous crop monitoring and precision interventions.
img: assets/img/1.jpg
importance: 1
category: work
---

> **Status:** [In progress / Completed] &nbsp;·&nbsp; **Timeline:** [Start date] – [End date] &nbsp;·&nbsp; **Role:** [Your role]

---

## Overview

[2–3 sentences describing the problem this robot solves. What gap does it fill? Who is the intended operator?]

[1–2 sentences on the outcome — what can the robot do, and why does it matter?]

<div class="row">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/1.jpg" class="img-fluid rounded z-depth-1" caption="[Robot in the field / System overview photo]" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/2.jpg" class="img-fluid rounded z-depth-1" caption="[Close-up / sensor pod / gripper]" %}
  </div>
</div>

---

## System Architecture

[1–2 sentences describing the high-level architecture — how the major subsystems fit together.]

{% include figure.liquid loading="eager" path="assets/img/3.jpg" class="img-fluid rounded z-depth-1" caption="[Block diagram or architecture overview]" %}

The system is broken into three primary layers:

- **Perception** — [Sensors used: cameras, LiDAR, GPS, IMU, etc. What they detect.]
- **Planning** — [How the robot decides where to go and what to do. Path planning algorithm, mission planner.]
- **Actuation** — [Drive system, end-effector or payload. How commands are executed.]

---

## Hardware

| Component | Part / Spec | Purpose |
|-----------|-------------|---------|
| Platform | [e.g., custom differential-drive frame] | Chassis and mobility |
| Compute | [e.g., NVIDIA Jetson Orin] | Onboard inference and control |
| Primary sensor | [e.g., Intel RealSense D435] | Depth + RGB perception |
| Localization | [e.g., u-blox F9P RTK GPS] | Centimeter-level positioning |
| Power | [e.g., 24V 20Ah LiFePO₄] | Runtime and load budget |

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/4.jpg" class="img-fluid rounded z-depth-1" caption="[Frame / chassis build]" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/5.jpg" class="img-fluid rounded z-depth-1" caption="[Electronics enclosure / wiring]" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/6.jpg" class="img-fluid rounded z-depth-1" caption="[Sensor suite / mast detail]" %}
  </div>
</div>

---

## Software & Autonomy Stack

[Brief description of the software environment — ROS 2? Custom framework? Language breakdown.]

### Perception

[How the robot sees the world. Detection model, trained on what data, running at what frequency.]

### Navigation

[Path planning approach. Local vs. global planner. How it handles obstacles or replanning.]

### Mission Management

[How tasks are defined and sequenced. Any state machine, behavior tree, or task graph.]

{% include figure.liquid loading="eager" path="assets/img/7.jpg" class="img-fluid rounded z-depth-1" caption="[Rviz visualization / software pipeline diagram]" %}

---

## Results

[What did you measure? What did the robot achieve in testing or deployment?]

| Metric | Result |
|--------|--------|
| Navigation accuracy | [e.g., ±3 cm cross-track error] |
| Detection precision | [e.g., 94% mAP @ 0.5 IoU] |
| Operational run time | [e.g., 4.5 hours per charge] |
| Area covered per run | [e.g., 0.8 acres] |

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/8.jpg" class="img-fluid rounded z-depth-1" caption="[Field trial photo]" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/9.jpg" class="img-fluid rounded z-depth-1" caption="[Data / output visualization]" %}
  </div>
</div>

---

## Challenges & Lessons Learned

- **[Challenge 1]** — [What went wrong or was harder than expected, and how you resolved it.]
- **[Challenge 2]** — [e.g., GPS multipath in row crops caused localization drift — solved by fusing wheel odometry with a Kalman filter.]
- **[Challenge 3]** — [What you would do differently if starting over.]

---

## Next Steps

- [ ] [Next milestone or open problem]
- [ ] [Planned hardware upgrade]
- [ ] [Software feature still in progress]
