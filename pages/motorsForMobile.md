---
title: Motors for Motorized Mobiles
layout: default
filename: motorsForMobiles.md
--- 
# About this page

This is a brief treatise on motors used to motorize art mobiles.

The previous pages discussed art mobiles and their motorization in general.
This page focuses on electric motors used in art mobiles.

## Basics of electric motors

This section provides general context.
It emphasizes practical motor characteristics relevant to art mobiles.

This section describes rotating electric motors that use electromagnetism.
Linear electric motors have a different construction,
which is not suited for art mobiles.
Some motors use electrostatic force,
but they are also not suited for art mobiles
since they require high voltages.

### Parts of an electric motor

An electric motor has a stator and a rotor.
The stator is usually the mounting surface of the motor.
The stator does not move.
The stator and rotor share an axis.

The rotor is commonly inside the stator.
A motor with the rotor inside the stator
is called an inrunner motor.
The shaft of the motor is fixed to the rotor,
concentric with the rotor
and through the rotor,
with a bearing on each end of the shaft.
One end of the shaft protrudes through a bearing
and connects to the load.

Some motors are dual-ended,
with the shaft protruding through both bearings, 
one on each side.

A motor with the rotor outside the stator
is called an outrunner motor.

### Kinds of electric motors

Rotating electric motors work by electromagnetic force.
The rotor and stator each provide a magnetic field
that interact by repelling and attracting each other.
One or both of the magnetic fields vary over time,
as the stator and rotor rotate in relation to each other.
After startup, at least one field is varied over time
to keep the poles of the two magnetic fields
pushing against each other.

Commonly, permanent magnets provide one of the magnetic fields.
But in induction motors,
one magnetic field induces a current and thus magnetism
in the other part (windings) of the motor.

### Methods of varying magnetic fields

Commonly, motors use brushes and commutator rings
to vary the magnetic field in the rotor.
In brushed motors, the brushes or bearings usually wear out
before faults in other components.

Brushless motors use electrical commutation.
BLDC is the abbreviation for "brushless DC."
Electronic switches vary the direction and timing of current to a set of coils.
The switches are commonly MOSFETs,
and a driver circuit controls the MOSFETs.
Integrated circuits are available containing both the MOSFETs and the driver circuit.

### Connection of an electric motor to its load

A typical electric motor is connected to a gear or pulley.
The gear is press-fit to the shaft,
or the shaft has a flat and the gear has a flat with a set screw.

### Axial loads

Most electric motors are designed for radial loads,
where the force of the load is orthogonal to the shaft.
Motors that are under axial load,
where there is a force in line with the shaft,
should have thrust bearings or washers.

### Starting torque

An electric motor requires more torque to start a load
turning than to keep the load turning.
This is called starting torque.
Often a motor must be unloaded for it to start properly,
and the load progressively applied.
A torsional element connecting a motor to its load
reduces the starting torque of the motor.

When an electric motor is stopped,
the mating surfaces of the bearings/bushings on the shaft
rest more closely together,
less separated by a film of oil,
with more friction.
This is called stiction.
More force is required to overcome this friction.

### Duty cycle

Motors generate heat.
The heat may build up if the motor is run continuously.
The motor may be destroyed by excess heat.
Motors can have a duty cycle rating
specifying whether they can be run continuously,
or only periodically.

### Stall current

The current to a motor whose shaft and rotor is locked and not turning
is called the stall current.
The stall current is more than the running current.
Stall current generates more heat than running current
and can destroy a motor.

## Considerations for electric motors used in mobiles

This section discusses unique requirements for typical uses of electric motors
in art mobiles.

### Brushed versus brushless

Brushed motors have a shorter life than BLDC motors.
Since art mobiles are difficult to reach to maintain,
it may be desirable to use long-life motors.

Brushed DC motors can be controlled by a single electronic switch.
A simple circuit can switch current to the low-side (ground side) of a DC motor.
This only controls whether the motor is on or off.
The speed of the motor is controlled by its voltage.
It adds complexity to also control the voltage.

BLDC motors add complexity to a motorized art mobile.
They require both a driver IC and a controller of the driver IC.
The driver IC lets you also control the speed of the motor.

### Voltage rating of motors in motorized art mobiles

It is more convenient to use low-voltage motors in art mobiles.
This is compatible with small solar cells, which are also usually low voltage.
A typical single solar cell produces 0.6 V.
A series of small solar cells can produce as much as 5 V.
The electronics to boost the voltage of solar cells add complexity to the design.

Small brushed DC motors are available that require as little as 1.5 V.
More common motors use 6 V.

BLDC motors are available that use as little as 3 V.
More common motors use 6 V.

### Choosing sizes for levels of motorized art mobiles

In a typical art mobile,
lower levels require less power.
Using a different motor size at each level adds complexity to the design.
Using the same size motor in each level
means some motors may have more power than needed.

### Axial load in motorized art mobiles

In a motorized art mobile,
a motor oriented shaft-up
axially carries the gravity load of the levels beneath it.
The radial load is the force to turn the level having the motor
plus the levels beneath it,
or at least to wind up a torsional element.

The axial bearing surfaces also suffer stiction.
The radial bearing surfaces may suffer less stiction.

### Starting torque

A torsional element connecting a motor in an art mobile
to the next level
reduces the starting torque of the motor.

### Duty cycle

Motors in a motorized art mobile usually run at a low duty cycle.
Buildup of heat is usually not a concern.

### Stall current

While motors in art mobiles may stall,
the motors are usually pulsed so that stall current is not sustained long,
and heat buildup is usually not a problem.