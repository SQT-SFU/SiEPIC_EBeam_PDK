# SiEPIC_EBeam_PDK

SiEPIC EBeam PDK, Library

Package for KLayout, klayout.de

by Lukas Chrostowski, (c) 2015

Developed on KLayout version 0.24.3, OSX.

##Package includes:

- PCells: ring resonator; test structure layout with grating couplers and instantiating the ring resonator
- Script / Macro to create a layout via script, including waveguide generation functions
- GDS Library, updated with marker layers for the verification/netlist generation.
- Verification and Netlist generation: 
 - Scanning the layout. Finding waveguides, devices, pins.  
 - Verification: Identifying if there are missing connections, mismatched waveguides, too few points in a bend, etc. 
 - Creating a Spice netlist suitable for importing into Lumerical INTERCONNECT for circuit simulations. Including waveguide length (wg_length) for all waveguides
 - Example layout using the library for verification.

## Download:

<a href="https://github.com/lukasc-ubc/SiEPIC_EBeam_PDK/archive/master.zip">Zip file download of the PDK</a>

This is posted on GitHub for 1) revision control, 2) so that others can contribute to it, find bugs, 3) easy download of the latest version.

##Installation instructions:

 - The files in the klayout_dot_config folder go into your KLayout configuration folder. On Linux and OSX, this is $HOME/.klayout
 - I don’t know what the equivalent is on windows. 
 - Alternatively, you can import all the files one by one using the KLayout IDE.  How to use the <a href = http://www.klayout.de/doc/about/macro_editor.html>KLayout Python IDE for writing/debugging PCells/scripts/macros</a>.

I am personally using GitHub desktop to synchronize my files. Then I created symbolic links in my .klayout folder to point to the local copy of this repository.


##Screenshots:

![Screenshot1](https://s3.amazonaws.com/edx-course-phot1x-chrostowski/PastedGraphic-9.png)
![Screenshot2](https://s3.amazonaws.com/edx-course-phot1x-chrostowski/PastedGraphic-10.png)
