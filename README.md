# Garbage Truck Tracking Simulation Program on Linux 🚛♻️🗑️
- Made with **advanced** data structers knowledge as a part of **CSE211** course
- Mostly C++ was used
- and little bit of MAKEFILE
## What does it do❓
- It simulates a garbage truck wandering around a city(grid) and loads garbage from the bins with critical level trash in it
- When the truck is fully loaded it needs to dispose so it goes to a disposal facility

```cpp
 if(truck.isFull()){
      int disposalLocation = planner.findNearestDisposal(currentLocation, facilities);

      if(disposalLocation != -1){
          distance = planner.computeDistance(currentLocation, disposalLocation);

          if(distance != INT_MAX && distance > 0){
              totalDistance += distance;
          }  

          truck.moveTo(disposalLocation);
          truck.unload();
          currentLocation = disposalLocation;
          }
      }
```
- And does this for 7 days
### On linux:
- All the info about the simulation is accessible by the user, like: Fill rates of bins and the garbage truck, grid map, success rate, simulation configuration panel, restart and start/pause button
- Also the speed of the simulation can be changed in order to take a close and detailed look on the program
