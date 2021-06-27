# GSRI-Skydiving

## What is GSRI Skydiving
This mod is a collection of small ajustments initially made for the french team [GSRI](https://www.gsri.team), revolving around skydiving in ArmA 3. Currently available features are detailed in the __Features__ section.

## Requirements
This mod requires [CBA](https://github.com/CBATeam/CBA_A3).

## Rules and standards
The following documents provide additional informations on rules and standards applying to this project :

*   [MIT License](../LICENSE)
*   [GSRI code of conduct](https://github.com/team-gsri/.github/blob/master/CODE_OF_CONDUCT.md)
*   [GSRI standard contribution guide](https://github.com/team-gsri/.github/blob/master/CONTRIBUTING.md)

## Features

### Newtonian free-fall

In vanilla ArmA 3, exiting an aircraft mid-flight will result in a physically speaking inconsistent behaviour. The velocity vector of the unit after exit is, at best, reset to `[0,0,0]`, and at worst set to some weird values in the direction opposit to aircraft's flight path.

The newtonian free-fall aims at correcting this by setting the velocity vector of units after exit on the same vector as the plane, exactly as natural laws of physics predict. Following this specific moment, the aircraft keep its velocity due to its engine compensating air friction, while free-falling units will slow down on the horizontal axis (due to air friction) while speeding up on the vertical axis (due to gravity), thus widening the gap between them and the aircraft.

This feature is strictly passive : as long as the `gsri_skydiving_enabled` setting is enabled in CBA settings