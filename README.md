[![Discord](https://img.shields.io/discord/616889479298547722?logo=discord)](https://discord.gg/P82fEmE)
[![License](https://img.shields.io/github/license/Open-RFlab/Open-RFlab)](LICENSE)

# Open-RFlab

## Description

A free & open source, complete, powerful and user friendly platform to design RF electronics. A real alternative to proprietary and onerous softwares. That is the Open-RFlab project's goal.

The actual FOSS electronics design environment is extremely heterogenous. It comes with its good softwares, its lacks and its incompatibilities. So most of the classic design workflows are difficult if not impossible, especially in RF.

The Open-RFlab project is about solving this situation. Not by creating The new perfect RF monolithic EDA, but 
by making existing softwares compatible with each other, easying their use, developing missing features and avoiding gaps in workflows. And an important one, by documenting what it is possible to achieve with such an ecosystem.

[CoralEDA](http://repo.hu/cgi-bin/pool.cgi?cmd=show&node=ecosys_prop) is a friend project from pcb-rnd guys. We share both goal and method to achieve it, except we are more focused on RF.

This is an early emerging project, help is welcome! :)

Feel free to join our [Discord[EN/FR]](https://discord.gg/P82fEmE).

Or to send an email : thomas.lepoix@protonmail.ch

## Our projects / TODO list

### [Qucs-RFlayout](https://github.com/thomaslepoix/Qucs-RFlayout) (Qucs -> PcbNew(KiCad) & OpenEMS) [Usable]

An interface to export microstrip Qucs schematics to KiCad layouts/footprints, pcb-rnd layouts and OpenEMS simulations. One of the easiest ways to perform FDTD on microstrip circuits.

### [oemsgen]() (OpenEMS script generator) [ASAP]

As the Qucs-RFlayout developer, I think that it is a good approach for a `somewhat2openems` converter to produce a whole script and not only an octave function containing shapes for example and letting the user write its script. The Qucs-RFlayout strength regarding other existing converters is the effort to provide a correct postprocessing and a correct script CLI. I'd like to extract this part of my code to a library and start collaborating with other project such as [pcbmodelgen](https://github.com/jcyrax/pcbmodelgen), [pcb-rnd](https://github.com/evanfoss/pcb2csx), [pyems](https://github.com/matthuszagh/pyems) or [this project](https://www.openems.de/forum/viewtopic.php?f=6&t=831&sid=1194aeef8461b6cde786fa41c02eb7c6).
That would lead to a more uniform OpenEMS interface from the user side and also open possibilities to wrap script execution in some GUI.

This will become soon an invitation to work together. :)

### [AlanSmithee](https://github.com/Open-RFlab/AlanSmithee) (Smith chart utility) [WIP]

Smith chart utility, Touchstone file reader. It is a beginning project.

### Ecosystem exploration [WIP]

Here is a list of some things looking interesting we need to investigate. It may result on a tutorial or a new project. Any user experience report on the items below or any pertinent thing would be welcome.

- [SCUFF-RF](http://homerreid.github.io/scuff-em-documentation/examples/YagiUdaAntennas/YagiUdaAntennas/) : gmsh compatible MOM solver. It seems to come out of the box for RF simulations (with excitation ports and S parameters output).

- KiCad -> [fcad_pcb](https://github.com/realthunder/fcad_pcb) -> FreeCAD -> [FEM Workbench](https://wiki.freecadweb.org/FEM_Install) : This workflow might lead to FEM simulation of circuits without so much effort.

### [Tutorials](tutorials/README.md) [WIP]

We have to group some existing tutorials and write some others, mostly about workflows involved in the RF electronics design procedure. And also about the tools usage, if what already exist is not clear enough.

### Helping [Qucs](https://github.com/Qucs/qucs) [TODO]

Qucs is currently surviving because active developers are too few to face the work quantity. If a C++/Qt developer with a lot of free time and experience in dealing with legacy code read this, here is a useful thing to do, the community would be so grateful. ;)

### Enhancing [OpenEMS](https://github.com/thliebig/openEMS) [TODO]

- The most important OpenEMS enhancement would be an automatic and performant mesher. Some existing tools already contain their own, maybe porting one to an Octave / Python function would be a good solution? Need discussion.

- Making the circuit design possible and user friendly trough appCSXCAD. [This project](https://www.openems.de/forum/viewtopic.php?f=6&t=831&sid=1194aeef8461b6cde786fa41c02eb7c6) is (was?) about that.

- Adding better and easier postprocessing functions. [Qucs-RFlayout](https://github.com/thomaslepoix/Qucs-RFlayout) ships reworked versions of `plotFF3D.m` and `plotRefl.m`.

## "Exhaustive" list of softwares compounding the ecosystem

TODO
