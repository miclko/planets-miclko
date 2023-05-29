# Planning document
Plan on how to create the program

## overview 

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
