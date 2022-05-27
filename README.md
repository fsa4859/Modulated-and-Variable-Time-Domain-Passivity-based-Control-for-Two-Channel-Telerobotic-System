# Modulated-and-Variable-Time-Domain-Passivity-based-Control-for-Two-Channel-Telerobotic-System
This project implements TDPC (Time Domain Passivity based Control), MDPC (Modulated Time Domain Passivity Control) and Variable Time Domain Passivity Control. The objective is to ensure the overall passivity and hence stability of the telerobotic system in the presence of communication delay and non passive flow of energy.

# TDPC 
## 
TDPC is a conservative approach that cancels any negative power backet being sent from the surgeon side to the patient's side.

## Resistive Behavior from Surgeon (Resistive Therapy)

### Simulink Model

![image](https://user-images.githubusercontent.com/69100847/170691961-563efb9e-f53e-43cb-914b-65f9b82e2093.png)


### Force Tracking

![image](https://user-images.githubusercontent.com/69100847/170692010-56a43192-1f28-424c-ae63-140379f0618f.png)


### Velocity Tracking

![image](https://user-images.githubusercontent.com/69100847/170692051-4e1c2cc5-229c-4473-a366-c74ca40d94eb.png)


## Assistive Behavior 

### Force Tracking

![image](https://user-images.githubusercontent.com/69100847/170692328-fae107fe-103d-46d8-a1b1-673a1525a829.png)


### Velocity Tracking

![image](https://user-images.githubusercontent.com/69100847/170692364-f877fc3a-0c6f-4cdc-96f4-9b1db56ead68.png)

It can be seen that since the surgeon provides assistive therapy, the TDPC control approach cancels out the assistive energy (non passive) to ensure the system stability. 

# MDPC

## Control Methodolgy

The MDPC takes into consideration the excess of passivity of the human biomechanics. It cancels only the non passive energy that can not be absorbed by the excess of passivity from the human biomechanics.

### Force Tracking

![image](https://user-images.githubusercontent.com/69100847/170693288-c7dd6281-fd97-4481-b095-9ae242bd7718.png)


### Velocity Tracking

![image](https://user-images.githubusercontent.com/69100847/170693329-6972c5b7-1cfd-4fbf-8886-d45797df23a5.png)


# VDPC

## 
The VDPC considers the variation of the excess of passivity during the system's operation.

### Force Tracking

![image](https://user-images.githubusercontent.com/69100847/170694435-ace4b334-9f60-4d68-8ebc-17e612e494ca.png)


### Velocity Tracking

![image](https://user-images.githubusercontent.com/69100847/170694497-ac4c171b-bdb2-4e3f-b146-5629c4f95e65.png)
