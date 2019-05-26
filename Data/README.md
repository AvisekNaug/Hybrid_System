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

### Possible alternative steps
* download the data upto april for room temp set points, energy data both heating and cooling, temp for the cct and dat as rest are useless, environmental data
* model the energy using these variables- use random shuffle to model the data vs contiguous shuffle
* make sure to model two different regimes
* Also see the variation in histogram variation in the weather data, sensor reading of temperatures, etc
* To calculate the heating energy, we need the flow values and supply return temps of hot water loop
* BEFORE! calculating or analyzing divide data into regions(based on temp+hum as well as valve op) otherwise sensor readings will not reflect what their actual prupose is.
* In bdx hw data, 0 values of flow corr to decereasing values of supply temp of hot water

* OR we can learn from the existin data about the HW energy given the setpoints of rooms, pht temps of ahus, dats of ahus and use it to predict the remaining cols
* THIS ^^ looks like a feasible thing to do!

