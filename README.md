# Mächtige Match Möve Marvin

## 🚁 Overview

**match Drohne** aka Marvin the Seagull.

![Marvin](marvin.jpg)


---

## 📦 Installation

### 1. Navigate to the `src` Directory

```bash
cd /path/to/your/ros2_ws/src
```

### 2. Clone This Repository

```bash
git clone https://github.com/Luca0204/Match-Drohne .
```

### 3. PX4 Setup (10–15 minutes)

```bash
git clone https://github.com/PX4/PX4-Autopilot.git --recursive
cd PX4-Autopilot
touch COLCON_IGNORE
DONT_RUN=1 make px4_sitl gazebo-classic_iris
```

### 4. Install MAVROS

```bash
sudo apt install -y ros-humble-mavros ros-humble-mavros-extras ros-humble-mavros-msgs
sudo apt install -y geographiclib-tools
sudo geographiclib-get-geoids egm96-5
```

---

## 🚀 Running the Demo

From the root of your workspace:

```bash
colcon build --symlink-install
source install/setup.bash
ros2 launch match_launch demo.launch.py
```

---


