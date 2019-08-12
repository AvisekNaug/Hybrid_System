# Analysis, modeling and control of HVAC system of a building under hybrid conditions

## Step1: Analyzing the total data to understand different relationships among energy and input variables

```
Data Hierarchy
Hybrid_System
|-SystemPictures
|-Data
|-src
```

*Next step is to read the data files for both AHUs(or just 1) and setpoints from zones*

## Apart from that I ran boosted regression on the entire data set and found the following independent variables to be affecting the chilled water energy consumption

  ```
  1. 'Condensor_Water_Loop_Valve.valvePosition'
  2. 'Primary_Chilled_Water_Valve.valvePosition'
  3. 'AHU_2.outdoorAirTemp'
  4. 'READING_ROOM_206_Indoor_Unit_89.spaceTemp'- Also space temperature from all zones were at the top
  5. 'Alumni_Hall_Cond_Loop_S_T.value'
  6. 'CC_T_2.value'
  7. 'WRITING_STUDIO_113_Indoor_Unit_20.localSetpoint'
  8. 'HX_Valve_1.valvePosition'
  9. 
  ```
  
  ## After this investigate whether the space temperatures are a function of the setpoints as modes moderated by outdoor temperatures
