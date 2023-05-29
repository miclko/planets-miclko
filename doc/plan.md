# Planning document
Plan on how to create the program

## overview 
The general structure of the program is given below. The functionality of the program can be split into three main topics
Creation of the initial parameters and number of planets. 
Simulation and storing of the evolution of the planets
Visualization of the dynamics

```PlantUML

@startuml
start
:Planet creator
Create initial positions and other parameters
for each planet;
:Simulation class
Evolve system from initial parameters
Create/store positions and velocities
Define simulation time
Physical constants (gravitational constant, masses)
Arbitrary planets;
:Store final positions;
:Process/plot data;
end
@enduml
```

## Needed parameters
The essential parameters are given by
  -  planet numberf (+ planet name)
  -  mass of planet
  -  choice of center of coordinate system (e.g. sun)
  -  positions
  -  velocities
  -  gravitational constant
    
## Development path

The program will be written in python.
It will use object oriented programming for the different parts

```python
class planet:
    def __init__(self, name, mass, position, velocity):
        self.__name = name
        self.__mass = mass
        self.__position = position
        self.__velocity = velocity
    def displace(self, displacement):
      ...
```
    
