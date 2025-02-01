# SnapWagon

# SnapWagon – User Flow Diagram

## Overview
SnapWagon is an **AR-powered driver assist system** using Snapchat Spectacles. This user flow outlines the major steps, from the first launch to the core experience.

## **User Flow Diagram**
The following diagram represents the user's journey through SnapWagon:

```mermaid
graph TD;
    A[User Starts SnapWagon] -->|First Time? Yes| B[Onboarding & Tutorial]
    A -->|Returning User| C[Main Dashboard]
    
    B --> D[Intro to AR Features]
    D --> E[Connect to Car Cameras]
    E --> F[Calibration & Setup]
    F --> G{Tutorial Completed?}
    
    G -->|Yes| C
    G -->|No| B

    C --> H{Choose Feature}
    H -->|Blind Spot Assist| I[Enable AR Alerts]
    H -->|Lane Assist| J[Activate Lane Detection]
    H -->|AR Navigation| K[Turn-by-Turn Directions]
    H -->|Parking Assist| L[Step-by-Step Parking Guidance]
    
    I --> M[Real-Time Blind Spot Detection]
    J --> N[Lane Departure Warning]
    K --> O[AR Navigation Overlay]
    L --> P[Parking Visualization]

    M --> Q[Driving Feedback & Stats]
    N --> Q
    O --> Q
    P --> Q
    
    Q --> R{Session Completed?}
    R -->|Yes| S[Show Driving Summary]
    R -->|No| H
    
    S --> T{Exit App?}
    T -->|Yes| U[End Session]
    T -->|No| C
```
## User Journey Breakdown

### 1. First-Time User
- User starts **SnapWagon** for the first time.  
- Walks through an **introductory AR tutorial**.  
- Connects to **car cameras via Wi-Fi/Bluetooth**.  
- Completes **calibration and setup**.  

### 2. Returning User
- User logs in and lands on the **Main Dashboard**.  
- Can select **AR features** such as:  
  - **Blind Spot Assist**  
  - **Lane Assist**  
  - **AR Navigation**  
  - **Parking Assist**  

### 3. AR Driving Assistance
- The Lens **detects vehicles, lane departures, stop signs**, and **projects AR alerts**.  
- **Real-time AR navigation overlays** guide the user.  
- Provides **audio warnings & haptic feedback**.  

### 4. End of Session
- The user receives a **driving performance report**.  
- Can choose to **restart** or **exit the session**.  

# SnapWagon – UI Structure Diagram

## Overview
This diagram represents the **UI flow and structure** of SnapWagon, outlining key screens and how users navigate through them.

```mermaid
graph TD;
    A[Welcome Screen] -->|New User| B[Onboarding & Setup]
    A -->|Returning User| C[Main Dashboard]
    
    %% Onboarding Flow %%
    B --> B1[Intro to SnapWagon]
    B1 --> B2[AR Tutorial: Lane Assist, Blind Spot Detection]
    B2 --> B3[Connect to Car Cameras]
    B3 --> B4[Calibration & Setup]
    B4 --> C

    %% Main Dashboard %%
    C -->|Select Feature| D{Feature Selection}
    D -->|Blind Spot Assist| E1[Enable AR Alerts]
    D -->|Lane Assist| E2[Activate Lane Detection]
    D -->|AR Navigation| E3[Turn-by-Turn Directions]
    D -->|Parking Assist| E4[Step-by-Step Parking Guidance]

    %% Feature Screens %%
    E1 --> F1[Blind Spot Detection Mode]
    E2 --> F2[Lane Departure Warning Mode]
    E3 --> F3[AR Navigation Overlay]
    E4 --> F4[Parking Visualization]

    %% Driving Feedback %%
    F1 --> G[Driving Performance & Feedback]
    F2 --> G
    F3 --> G
    F4 --> G

    %% Session End Flow %%
    G --> H{End of Session?}
    H -->|Yes| I[Driving Summary Report]
    H -->|No| D

    I --> J{Exit App?}
    J -->|Yes| K[End Session]
    J -->|No| C
```
## UI Structure Breakdown

### 1. Welcome Screen
- **New Users** → Onboarding, tutorial, and initial setup.  
- **Returning Users** → Go directly to the **Main Dashboard**.  

### 2. Onboarding & Setup
- **Intro to SnapWagon’s features**.  
- **Walkthrough of AR tutorials**.  
- **Connect to car cameras & perform calibration**.  

### 3. Main Dashboard
- Central hub for selecting **driving assistance features**:  
  - **Blind Spot Assist**  
  - **Lane Assist**  
  - **AR Navigation**  
  - **Parking Assist**  

### 4. Core Features
- **Blind Spot Detection Mode** → AR overlay alerts.  
- **Lane Departure Warning Mode** → Lane assist indicators.  
- **AR Navigation Overlay** → Turn-by-turn guidance.  
- **Parking Visualization** → Step-by-step parking assistance.  

### 5. Driving Feedback & End of Session
- User receives a **performance report**.  
- Option to **restart another session** or **exit the Lens**.  

# Lo-Fi Wireframes for SnapWagon's Key Screens

## Welcome Screen
- **SnapWagon logo**  
- Options for **Login** or **Guest Mode**  

## Main Dashboard
- **User Profile**  
- Central hub to select features:  
  - **Blind Spot Assist**  
  - **Lane Assist**  
  - **AR Navigation**  
  - **Parking Assist**  

## AR Feature Screen (Blind Spot Detection)
- **Live camera feed** from car  
- **AR overlay** showing detected vehicles in blind spots  
- **Warning alert** in case of close proximity  

## Driving Feedback Screen
- **Trip Summary**  
- **Score & badges earned**  
- Options to **restart session** or **exit**  

![image](https://github.com/user-attachments/assets/d549047e-54cf-48f9-ba32-6e7b274ef03f)
