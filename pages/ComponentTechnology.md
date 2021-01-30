---
title: Components I use in Solabiles
layout: default
filename: ComponentTechnology.md
--- 
# Components I use in Solabiles

This about the manufacturers of electronic and other parts.

Also some considerations for selecting parts for ultra-low, solar power.

I use mass-produced parts that are available retail or on-line.
I try not to use special, hard-to-find, unobtainable parts.

## Solar Cells

I often use glass, indoor solar cells from [Panasonic Amorton.](https://panasonic.co.jp/ls/psam/en/products/pdf/Catalog_Amorton_ENG.pdf)
These are the same as used in solar calculators.
They are intended for indoor light.

I also use film solar cells from [Powerfilm](https://www.powerfilmsolar.com/) that are printed on rollers.
Most of them are intended for outdoor, sunlight.
But their new models such as LL3-37 are better in indoor light.

I also use [IXYS](https://ixapps.ixys.com/DataSheet/IXYS%20Solar%20Product%20Brief.pdf) solar cells for sunlight.

All are available from Digikey.

Sometimes I use a blocking diode on the solar cell.
I don't when the use case is "there's enough light or there isn't."
When the use case is "store energy for dark periods"
I either use a blocking diode,
or a energy harvester that effectively blocks leakage
in the reverse direction through the solar cell.

## Motors

For my small works, I use pager motors.
They are inexpensive, and readily available.
They are inexpensive because billions are used to vibrate cell phones.
They are [brushed DC motors](https://en.wikipedia.org/wiki/Brushed_DC_electric_motor)
that operate down to one volt and a hundred milliamps.

Brushed motors require no special circuitry to drive them.
That is, the power is either on or off.
I usually use an NMOS [power mosfet](https://en.wikipedia.org/wiki/Power_MOSFET)
to switch the low side (switched ground.)

I sometimes use [brushless (BLDC) motors](https://en.wikipedia.org/wiki/Brushless_DC_electric_motor).
They usually require driver chips to operate them.
But they have an expected lifetime longer than that of brushed motors.

Some motors used in flying drones are brushless and inexpensive, from China.

[Faulhaber](https://www.faulhaber.com/en/home/),
[Maxon](https://www.maxongroup.com/maxon/view/content/index),
and [Nidec](https://www.nidec.com/en/)
make brushless motors.

## Integrated circuits

I often used IC's from [Texas Instruments](https://www.ti.com/)

Solar energy [harvesters.](https://en.wikipedia.org/wiki/Energy_harvesting)

Motor drivers or [controllers](https://en.wikipedia.org/wiki/Motor_controller).

Voltage monitors or PMICs.

Load switches (a sophisticated electronic switch.)

## Capacitors

I don't use batteries, only capacitors, 
which have a much longer lifetime (many decades)
and are not a chemical or fire hazard.

When I need a small capacitor, I use [tantalum capacitors](https://en.wikipedia.org/wiki/Tantalum_capacitor).
They have a high density (high volumetric capacitance.)

When I need more capacitance (say for a large motor or to store energy overnight) 
I use [super capacitors.](https://en.wikipedia.org/wiki/Supercapacitor)

For the application of ultra-low, solar power,
the leakage (DCL) of the capacitor dominates the [leakage](https://en.wikipedia.org/wiki/Leakage_(electronics))
of other components such as switches.
The capacitors must be "low leakage."

For the application of driving motors,
the capacitors must provide a high current pulse.
The capacitors must be low [ESR](https://en.wikipedia.org/wiki/Equivalent_series_resistance).




