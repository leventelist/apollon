# apollon
Printed Circuit Board editor.


Hystory
=======

While I was in the air traveling to/from Greece, I decided to write a new data
structure for gEDA/PCB. Not because it is unusable, but I wanted to have one
place for the layout data, and other attributes, like mechanical data,
schematic symbol. The whole thing stared out as a small parser of pcb files
that puts everything to an SQLite database.

After a while an idea came that what I was really doing, is defining a new
data structure and file format for pcb. My mind went further, and realised
that the current gEDA/pcb lacks lots of feature, and a new tool must be
created to be able to achieve the goals of a professional EDA tool.

In Greek mythology, Aplollo is the God of knowledge, music, art and healing.
Apollon is how Hungarian people spell Apollo. I hope this tool will help
engineers to create their professional PCB layouts while enjoying the beauty
of Apollon.


Contributors needed
===================

I need contributors who help me write this code. I want to use as much code
from gEDA/pcb as I can. However I want the following features to be
implemented on the top of current pcb functionality.

 * The user can edit footprints by using the GUI.
 * The user can draw arbitrary padstacks.
 * No concept of footprint, just embedded layouts.
 * Blind and buried VIAs


What we have today
==================

 * We have a data structure and SQL schema.
 * A perl script that reads a gEDA/pcb file and builds up a database form it.


That is not much, I know.


Roadmap
=======

 * Write a parser of the data structures
 * Write an engine that can display primitive shapes
 * Either weld this to gEDA/pcb, or create a new tool
 * The rest will come :-)

Technology
==========

 * SQLite for data storage
 * FLTK for the GUI toolkit
 * git for VCS.
 * Cmake for configuration management
 * C++


Author
======

leventelist@gmail.com

I hope more will join.

