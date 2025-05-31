# CMI - Detect Behavior with Sensor Data

## 🧠 Overview

Can you use movement, temperature, and proximity sensor data to differentiate between body-focused repetitive behaviors (BFRBs), like hair pulling, from non-BFRB everyday gestures, like adjusting glasses?

This competition challenges participants to develop a predictive model that distinguishes BFRB-like activity from non-BFRB-like activity using data from a variety of sensors collected via a wrist-worn device. Successfully distinguishing these behaviors will inform the design and accuracy of wearable BFRB-detection devices, which are crucial in diagnosing and supporting mental health treatments.

---

## 📖 Description

**Body-focused repetitive behaviors (BFRBs)** — such as hair pulling, skin picking, and nail biting — are self-directed repetitive habits that may cause physical harm and psychosocial challenges. These behaviors are often associated with anxiety and obsessive-compulsive disorders.

To investigate BFRBs, the **Child Mind Institute** has developed a wrist-worn device called **Helios**, designed specifically to detect such behaviors.

### Helios Device Features:

- **IMU (Inertial Measurement Units)** for measuring rotation and motion.
- **5 Thermopile Sensors** to detect body heat.
- **5 Time-of-Flight Sensors** to detect proximity.

---

## 🧪 Study Design

Participants wore the Helios device and performed a sequence of repeated gestures involving:

1. **Transition**: Moving hand from a rest position.
2. **Pause**: A short break doing nothing.
3. **Gesture**: Performing either a BFRB-like or non-BFRB-like movement.

Each participant performed **18 unique gestures** (8 BFRB-like and 10 non-BFRB-like) in at least one of the following **four body positions**:

- Sitting
- Sitting leaning forward (non-dominant arm on leg)
- Lying on back
- Lying on side

---

## ✋ Gesture Categories

### ✅ BFRB-Like Gestures (Target Gestures)

| Gesture                        | Position(s) Performed        |
|-------------------------------|------------------------------|
| Above ear - Pull hair         | Sitting                      |
| Forehead - Pull hairline      | Sitting leaning forward      |
| Forehead - Scratch            | Sitting                      |
| Eyebrow - Pull hair           | Sitting                      |
| Eyelash - Pull hair           | Sitting                      |
| Neck - Pinch skin             | Sitting                      |
| Neck - Scratch                | Sitting                      |
| Cheek - Pinch skin            | Sitting, Leaning, Back, Side |

### ❌ Non-BFRB-Like Gestures (Non-Target Gestures)

| Gesture                                 | Position(s) Performed       |
|----------------------------------------|-----------------------------|
| Drink from bottle/cup                  | Sitting                     |
| Glasses on/off                         | Sitting                     |
| Pull air toward your face              | Sitting                     |
| Pinch knee/leg skin                    | Sitting leaning forward     |
| Scratch knee/leg skin                  | Sitting leaning forward     |
| Write name on leg                      | Sitting leaning forward     |
| Text on phone                          | Sitting                     |
| Feel around in tray and pull object    | Sitting                     |
| Write name in air                      | Sitting                     |
| Wave hello                             | Sitting                     |

---

## 🎯 Challenge Objectives

- **Binary Classification**: Detect if a gesture is BFRB-like or not.
- **Multiclass Classification**: Identify the specific type of BFRB-like gesture.

### ⚠️ Evaluation Constraint:
Half of the test set includes **IMU-only data**, and the other half includes **full sensor data (IMU + thermopiles + ToF sensors)**.

---

## 🌍 Real-World Impact

Your models will inform design choices in wearable sensor technology by evaluating:

- **Does adding thermopile and time-of-flight sensors significantly improve detection?**
- **Can we build accurate, affordable BFRB detection tools?**

Improved accuracy and affordability could transform how mental health conditions involving BFRBs are monitored and treated.

---

## 🔗 References

- [What Is Excoriation, or Skin-Picking? – Child Mind Institute](https://childmind.org/article/excoriation-or-skin-picking/)
- [What is Trichotillomania? – Child Mind Institute](https://childmind.org/article/what-is-trichotillomania/)
