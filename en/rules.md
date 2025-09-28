---
title: ROBORACER GRAND PRIX Rules
layout: page
section: race
language: en-US
base_url: rules.html
---

<style>
.post ol {
  list-style-type: lower-alpha;
}

.post ol ol,
.post ul ol {
  list-style-type: lower-roman;
}
.post ol, .post ul, .post p {
  margin-bottom: 0rem;
}
h2, h3, h4, h5, h6 {
  margin-top: 1rem;
  margin-bottom: 1rem;
}
</style>

*Last Updated: 2025-09-28*

<!-- *수정일자: 2022-10-15* -->

<!-- 
1. Video submission 
1.1 Video submission exmaple
2. Car inspection - chassis, tires, detection box, foam bumper, motor. battery, main computation unit, lidar, camera, other sensors
3. mapping & practice, mapping, regulated practice, open practice
4. rules 
4.1 Rules for Qualifying and Head-to-head
All computations must be performed onboard!!
No protests regarding Wi-Fi will be accepted.
● Strictly prohibit manual (human) emergency brake
● No data must be transmitted to the vehicle during the race.
Exceptions
  Joystick
    At the start or re-start(for start)
    For emergency stop (ex. After crash, reverse driving, remaining stuck in an obstacle for more than 5
    seconds)
    For entering Pit-stop zone on the Manual Drive Zone for pit-stop
  Remote computer
    When your car is out of track
    When your car is in pit-stop region
    When your car needs re-localization(only for giving initial-guess to your localization algorithm)
Pit-stop
Re-entering
● Any H/W repairment & maintenance inside the track is prohibited (not even pit-stop).

5. Phase 3: Qualification
● Time Trials
● Two goals (two leaderboards):
6. Phase 4: Head-to-head race
● Head-to-head Race
● Random Static Obstacle Areas
Crashing
Penalty cases in Head-to-head race
Warning cases in Head-to-head race

7.Key Point Summary
 -->
 
**Table of content**
- ToC
{:toc}


# 1. Overview

International ROBORACER Autonomous Racing Competition is a racing competition open to teams of all levels. Competing teams may consist of any number of members; however, each participant should be **a member of only one team**.

This competition will be held as an in-person competition from **August 24th (Monday)** to **August 27th (Thursday)**, **2026**, at **BEXCO** in Busan during **IFAC 2026** (The International Federation of Automatic Control).

ROBORACER Autonomous Racing Competition Schedule: **August 24th (Monday) ~ 27th (Thursday), 2026**

Teams can **register** for the competition through the **official website.** 

<!-- The preferred communication method with the organizers is the ICCAS2024 channel on [ROBORACER GRAND PRIX-teams Slack](https://join.slack.com/t/f1tenthxkorea/shared_invite/zt-1ibqf5yjq-CkG_z1XRhsZgBsCoSy7JiA). -->


# 2. Competition General

1. The competition consists of 4 phases:
  - **Phase 0**: Video submission demonstrating obstacle avoidance capability
  - **Phase 1**: Registration and inspection
  - **Phase 2**: Mapping and practice sessions (mapping, regulated practice, open practice)
  - **Phase 3**: Qualification (time trials)
  - **Phase 4**: Head-to-head race

2. Teams registered for in-person competition must provide and build their own vehicles according to the constraints listed below. Additionally, each team must have a unique vehicle (i.e., one lab cannot register six teams with one vehicle).

3. To improve the quality of future ROBORACER competitions, winners of each race are encouraged to open-source their algorithm code under an open-source license in the [ROBORACER Autonomous Racing Community repository](https://github.com/f1tenth) on Github.

## 2.0 Video Submission

1. Teams must submit a video demonstrating obstacle avoidance capability before the competition.

2. No specific format is required.

3. The submission must demonstrate the vehicle completing **more than two laps** on the track while **avoiding static or dynamic obstacles**.

4. Due date is Oct. 31th and submit to **uj7050@gmail.com**.

5. Please adhere to the deadline.

## 2.1 Vehicle Specifications
**Vehicle Specifications** only allows vehicles that meet the following constraints:

  <!-- 1. The vehicle is constructed according to the official [bill of materials](https://f1tenth.readthedocs.io/en/stable/getting_started/build_car/bom.html). The teams are allowed to use components of similar or lower specifications. -->

  1. Vehicles must be built according to ROBORACER guidelines, but alternative parts may be allowed as long as they comply with regulations. Unclear or ambiguous items must be confirmed in advance with race organizers.
  2. Each vehicle is inspected as part of qualifying to determine if it meets criteria. If criteria are not met, the vehicle cannot participate.
  3. **The ROBORACER Autonomous Racing Competition emphasizes algorithmic performance. Hardware designed to provide an unfair advantage is strictly prohibited.**.
  4. _Chassis_:
    The race is designed for **1:10 Traxxas** chassis (e.g., TRA74054, TRA6804R). While these chassis are recommended, chassis generally within 15% of Traxxas vehicle dimensions are allowed (238mm ≤ width ≤ 341mm, 454mm ≤ length ≤ 654mm). Both **4WD and 2WD** are allowed.
  5. _Tires_:
    **No limitations** (both sponge and rubber allowed). However, **chemical additives are strictly prohibited**.
  6. _Main Computing Unit_:
    **No limitations** on specifications. Only one computing unit may be used.
  7. _LiDAR_:
    **No limitations** on specifications. Only one LiDAR sensor may be used. **3D LiDAR** is allowed for this competition.
    (Note that expensive 3D LiDAR may be damaged in high-speed racing).
  8. _Camera_:
    Both **single cameras** (e.g., Logitech C270, Logitech C920, Raspberry Pi Camera Module V2, Arducam) and **stereo cameras** (e.g., Intel Realsense, ZED) are allowed. Cameras that provide additional information such as **detection or VIO results** from internal camera processing are **not allowed**. (Depth information is allowed)
  9. _Motor_:
    **No limitations** on specifications. Only a **single motor** may be used in the powertrain.
  10. _Battery_:
    **4s LiPo battery** or **3S or lower**. Only one 4S battery or lower cell combinations allowed (e.g., 2s + 2s allowed).
  11. _Detection Box_:
    Vehicles must be easily detectable by opponents' LiDAR. Therefore, vehicles must occupy at least **12×12cm** space on all horizontal planes between **10-30cm** from the ground.
  12. _Foam Bumper_:
    Bumpers must be soft to minimize damage. These two components (detection box and foam bumper) must be attached when there are two or more vehicles on the track.
  13. _Other Sensors_:
    Other sensors (IMU, encoders, custom electronic speed controllers) are allowed. Indoor GPS sensors (e.g., Marvelmind) are **not allowed**.

## 2.2 Track and Racing Environment

The competition will be held at Songdo Convensia in Incheon. The characteristics of the environment where the track will be built are:
- The track size is 20x10m.
- The surface is carpeted material.
<!-- 1. The surface is flat and reflective. Therefore, LiDAR beams may reflect from the ground and measure the surrounding area rather than the ground. Similarly, depth cameras have problems with proper ground detection.
2. The room is surrounded by windows and “glass walls”. The windows will be covered by non-transparent material up to 50 cm from the ground to improve the perception. The room is bright, and the Sun can shine into it.
3. The track border is constructed from one air pipes of 33 cm diameters. They are made from aluminium and metal, secured with plastic/wodden holders. Keep in mind that there can be a gap between the pipes through which the LiDAR beams can pass.
4. The track will fit into the area of around the size of 25×10 m.
5. The track can be mapped in either the training sessions on each day or in the qualification session of each team. We are not providing a dedicated time slot for teams to map the track. Since many teams using SLAM algorithm or vision-based localization techniques, a dedicated **Map Creation** or **Mapping** session is not provided for the teams. -->

<!-- 1. The surface is flat and covered with rugs. 
2. The room is a segmented space that uses a gable wall for parts of the auditorium. Since there is no window on the wall, there is no external light coming in, and it is all composed of non-transparent materials.
3. The track border is constructed from one air pipes of 50 cm diameters. They are made from polyester and metal, secured with cable tie and masking tape. Keep in mind that there can be a gap between the pipes through which the LiDAR beams can pass.
5. We will allocate a **mapping** time slot for each team approximately for 5 minutes, depending on the scale of the competition. -->

## 2.3 Inspection

- The purpose of inspection is to verify that autonomous vehicle hardware meets competition requirements and is not dangerous to the environment, opponents, or people.
- Vehicles must be built according to ROBORACER guidelines, but alternative parts may be allowed as long as they comply with regulations.
- Teams must demonstrate the ability to activate emergency brakes through remote human control (but **cannot be used for intervention during racing**!).
- Vehicle inspection is conducted on the first day of the competition.
- Inspection is performed by race referees.
- Inspection must be completed **before time trials** and after **significant changes** to vehicle hardware or algorithms.

## 2.4 Mapping and Practice

### 2.4.1 Mapping
- Each team is given approximately 5 minutes.
- This is time when one team can exclusively use the entire track.
- This time can be used not only for mapping but also for data acquisition and practice.
- If you miss your designated time slot, the opportunity is lost and no additional time is provided.
- Each team may prepare and use multiple vehicles on the track.
- Teams without map files are allowed to receive them from neighboring teams, but organizers will not assist with this.

### 2.4.2 Practice
- Consists of **Group practice** and **Open practice**.
- Each team may prepare multiple vehicles, but only one vehicle per team may be on the track.
- Sample obstacles are provided.
- No responsibility is taken for accidents that occur during practice.
- However, teams involved in accidents must explain their algorithms when requested by referees.

## 2.5 Pit Stop
<center>
<img src="../images/rules/pitstop.png"  style="width: 17vw" />
</center>

### 2.5.1 General
- This area is designated for parameter tuning **without removing vehicles from the track**.
- This area can be used in both qualifying and head-to-head racing.
- When a vehicle is in the **pit stop zone**, computers (mouse and keyboard) may be used for repositioning and parameter updates.
- As with the general track, people are prohibited from standing in this area.
- Additionally, after safely entering this area, taking out the vehicle to the island for repairs is not regarded as a warning situation.
- Using this area during autonomous racing mode is prohibited.

### 2.5.1 Entry
- Manual driving can only be used to enter the pit stop zone from the **manual driving area**.
- Manual driving to enter the pit during head-to-head racing **must not harm** the opponent's vehicle.

### 2.5.2 Exit
- **Do not manually drive in any way** when exiting from the pit stop zone to the general driving area.
- Vehicles exiting from the pit stop zone to the general driving area have an obligation to protect vehicles in the general driving area.

## 2.6 Qualifying (Time Trial)
<center>
<img src="../images/rules/qualification.png"  style="width: 20vw" />
</center>

### 2.6.1 General
- Both practice and qualifying use the same track.
- Conducted for **4 minutes** out of the given 6 minutes.
  - Qualifying can start anytime within 6 minutes, but 4 minutes is not guaranteed.
  - May change depending on total number of participating teams.

### 2.6.2 Objective
- Fastest **lap time**
- **Maximum number of laps** completed without collision
- Two records are ranked separately, then combined to determine final qualifying results.

### 2.6.3 Static Obstacles
- One **static obstacle** is randomly placed in each obstacle area.
- Each obstacle is smaller than 0.5m x 0.5m.
- Obstacle positions are announced on the morning of qualifying day and apply equally to all teams.
- **Obstacles are removed midway through qualifying time.** (e.g., if 4 minutes, removed after 2 minutes)
- Obstacles are safely removed when vehicles are not affected.

### 2.6.4 Record Invalidation
- **Invalidates lap time** and **resets completed lap count** if human intervention affects the vehicle.
- **Invalidates lap time** and **resets completed lap count** if contact occurs with static obstacles.
- If contact with track occurs but driving is possible without human intervention, it is considered minor contact and records remain valid.

### 2.6.5 Precautions
- Taking vehicles to **arbitrary positions (e.g., starting line)** during qualifying is **strictly prohibited**.
- If a vehicle is removed from the track and replaced for any reason, the vehicle direction can be slightly adjusted but must be placed back at the **position where it exited**.
- If track contact occurs, even if records are not invalidated, **the track must immediately be returned to its original position**.
- If obstacle contact occurs, it must immediately be returned to its original position.
- **All computation must be performed inside the vehicle!!**
- **Data must not be transmitted to vehicles during normal driving.**
- **Manual (human) emergency brakes are strictly prohibited during normal driving**
- There are 2 islands in the track and 2 people can be on one island.
  - People will be on islands in the following configuration: (Referee1, Team member1 from Team1), (Referee2, Team member2 from Team1)

## 2.7 Head-to-Head Racing
<center>
<img src="../images/rules/head_to_head.png"  style="width: 13vw" />
</center>

### 2.7.1 General
- Two vehicles start from different starting lines positioned in opposite directions.
- A total of two static obstacles are used. After all teams complete race preparation, one obstacle is randomly placed in each area.
- Static obstacles on the track are removed sometime after the race starts.
- Each vehicle must complete 20 laps first while avoiding obstacles and opponents within the time limit.
- Racing starts no later than 10 minutes after start preparation begins, regardless of both teams' readiness.

### 2.7.2 Objective
- Complete 20 laps first.

### 2.7.3 Random Static Obstacles
- One **static obstacle** is randomly placed in each obstacle area.
- Each obstacle is smaller than 0.5m x 0.5m.
- Obstacle positions are determined after both vehicles are ready at their starting lines.
- Only after obstacles are placed can start signals be transmitted to vehicles.
- **Obstacles are removed midway through the race.**
- Obstacle removal time is (average of best qualifying records of both teams) x 20 / 2.
- Red square areas indicate where static obstacles can be placed.
- Obstacles are safely removed when both vehicles are not affected.

### 2.7.4 Collisions
- Track boundaries and static obstacles
  - Restore track and obstacles
  - If racing can continue, it must continue without interruption.
- Vehicle to vehicle
  - **Do not stop racing at team discretion without referee's stop signal!!**
  - If the offending vehicle is clear in a collision situation but fails to overtake, the race continues as is.
  - If the victim vehicle is clear in a collision situation and the victim vehicle cannot drive or the collision is serious or gets overtaken, the race is stopped.

### 2.7.5 Precautions
- **Do not stop racing at team discretion without referee's stop signal!!**
- **All computation must be performed inside the vehicle!!**
- **Data must not be transmitted to vehicles during normal driving.**
- **Manual (human) emergency brakes are strictly prohibited during normal driving**
- Vehicles with detection boxes that violate regulations cannot participate in the race.
- There are 2 islands in the track and 2 people can be on one island.
  - People will be on islands in the following configuration: (Referee1, Team member from Team1), (Referee2, Team member from Team2)
- Contact and accidents while running side by side will not stop the race if there is no clear offender.

## 2.8 Common Precautions (Important!!)
- If driving becomes difficult or dangerous due to collision, the vehicle must be emergency stopped immediately.
- **All computation must be performed inside the vehicle!!**
- **Data must not be transmitted to vehicles during normal driving.**
- **Manual (human) emergency brakes are strictly prohibited during normal driving**
- Each team may prepare multiple vehicles, but the only time more than 2 vehicles from the same team can be on the track is during mapping time.
- Sharing one vehicle among multiple teams is strictly prohibited.
- If there can be 2 or more cars on the track, detection boxes must be attached. (e.g., not required for mapping or qualifying)
- **No complaints about Wi-Fi will be accepted.** Please ensure your autonomous driving system is designed to operate independently regardless of Wi-Fi conditions. We will ask non-racing teams to turn off their Wi-Fi, but this is purely to facilitate team visualization and debugging, not for algorithm performance!
- All hardware repairs and maintenance inside the track (repairing broken components, sensor recalibration, battery replacement, etc.) are prohibited. (Not allowed even in pit stop area)
- Dedicated time for **mapping**, **official practice**, and **qualifying** may vary depending on the number of participating teams.
- Dedicated time for **mapping** and **official practice** sessions is assigned on a **first-come, first-served basis** and only teams that have **successfully completed registration and inspection** are eligible.
- People are prohibited from being on the track. (Except during mapping time)
- **Use** of joystick or **pressing** joystick during racing is **not allowed**.
- Please change the module for autonomous driving <-> human control switching from "**press and hold**" method to "**on/off**" **toggle** method.
- Only one laptop may be connected for visualization (e.g., RViz) or debugging purposes.
- If space is needed because the vehicle is stopped too close to front obstacles (opponent vehicle or static obstacles) making evasive maneuvers impossible, you can request the referee to move it back slightly.

# 3. Warnings and Penalties
- **Decisions on incidents are at the discretion of on-site referees and must be respected.**
- Even incidents with **multiple violations** only apply **one penalty per incident**
## 3.1 Qualifying
### 3.1.1 One Rank Demotion
- Using keyboard or mouse during racing
  - Keyboard and mouse use prohibited even if no data transmission occurs
  - Exception 1: When vehicle is not on track
  - Exception 2: When on pit stop section
  - Exception 3: When transmitting initial guess for re-localization
- Manual manipulation (joystick, keyboard, or other devices) interfering with own vehicle
  - Exception 1: When emergency stop is needed due to referee declaring race stoppage
  - Exception 2: When transmitting start signal at start/restart
  - Exception 3: When emergency stop is needed due to inability to drive from collision
  - Exception 4: For manual driving in pit stop manual driving area to enter pit stop section
  - Exception 5: When emergency stop is needed after being trapped by obstacles for more than 5 seconds
  - Exception 6: When emergency stop is needed to prevent abnormal driving (sudden acceleration, reverse driving, etc.)
  - Exception 7: When referee allows manual manipulation because opponent vehicle seriously damaged track making driving impossible
  - Exception 8: When stopping after qualifying ends
- **During racing**, when humans directly generate or select modified paths based on obstacle positions

## 3.2 Head-to-Head Racing
### 3.2.1 Additional 1 Lap
- When 3 warnings accumulate
- Human's **fatal interference** with opponent vehicle during racing
  - When going to fix track causes physical contact with opponent vehicle affecting driving
- When clear offending and victim vehicles exist and victim vehicle becomes unable to drive
- **Complete rear collision with large impact accident**
- **Even if not complete rear collision, accident with large impact**
- Using keyboard or mouse during racing
  - Keyboard and mouse use prohibited even if no data transmission occurs
  - Exception 1: When vehicle is not on track
  - Exception 2: When on pit stop section
  - Exception 3: When exiting track and re-entering, transmitting initial guess for re-localization
- Manual manipulation (joystick, keyboard, or other devices) interfering with own vehicle
  - Exception 1: When emergency stop is needed due to referee declaring race stoppage
  - Exception 2: After start, restart, end
  - Exception 3: When unable to drive due to collision
  - Exception 4: For manual driving in pit stop manual driving area to enter pit stop section
  - Exception 5: When stopping for manual manipulation change after being trapped by obstacles for more than 5 seconds
  - Exception 6: When emergency stopping to prevent abnormal driving (sudden acceleration, reverse driving, etc.)
- **During racing**, when humans directly generate or select modified paths based on obstacle positions

### 3.2.2 Warning 1 Time
- False start
- Not actively restoring track
- Completely crossing pit stop zone in autonomous racing mode
- Detection box not properly secured during race
  - Exception 1: When fixed and running in pit stop zone within 1 lap after warning
  - New warnings can be given for each lap not properly fixed
- **Intervention** with own vehicle during racing
  - Removing vehicle outside track after collision
  - Directly modifying vehicle heading
- Human **interference** with opponent vehicle during racing
  - When going to fix track gets detected by opponent vehicle's detection module affecting driving

### 3.2.3 Example Cases
<center>
<img src="../images/rules/crash1.png"  style="height: 18vw" />
</center>
<center>
<img src="../images/rules/crash2.png"  style="height: 18vw" />
</center>