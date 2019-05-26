# Dataset Description

## Raw Data Files

* TotalEnergy2018- Has the heating and cooling energy data, ambient data and hot water data
* ORH- Has the Relative humiditysince Alumni Hall sensoris not working right now

### Update: Baesd on looking at the CHW.xlsx data, 
* Either the reheat, cool outputs are depending on the diff of temp set pt and the actual temp because dehum command are
not governing what is happening to the cooling and heating process it seems. Have to check!
* Observation 1: The reheat section works based on whether the actual disc temp is > set pt so pretty logical
* However, can't seem to understand how the cooling works. Have to ask Darren

The cooling output is suddenly zero, when the outside temperature in the 80s and the humidity is in the 70s while the 
cct is in the 70s