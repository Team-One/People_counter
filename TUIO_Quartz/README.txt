TUIO Quartz Composer Plugin
---------------------------
Copyright (c) 2005-2009 Martin Kaltenbrunner <mkalten@iua.upf.edu>
This software is part of reacTIVision, an open source fiducial
tracking and multi-touch framework based on computer vision. 

http://reactivision.sourceforge.net/

Many thanks to Sandor Rozsa <rozsa@cd-cologne.de>
for providing the basis for the improved TuioDemo patch.

Installation:
-------------
Copy the Quartz Composer Plugin "TuioClient.plugin" into the folder
"/Library/Graphics/Quartz Composer Plug-Ins/" and restart Quartz Composer.

Demo Patch:
-----------
This package contains a basic Quartz Composer patch "TuioDemo"
that receives and decodes TUIO messages reveived from any TUIO enabled
tracker. This patch draws a black square along with the SymbolID
for any received TuioObject as well as a grey circle for each TuioCursor.

The TuioClient Plugin has a settings field for an optional UDP port.
The default TUIO UDP port is 3333.

There are two outputs, the first one is giving all current TuioObjects,
while the second  port outputs TuioCursors. Both ports output "Structures",
which are parameter lists, containing the following fields:

s_id ... session ID
c_id ... cursor ID / symbol ID
xpos ... position on X-axis (0...1)
ypos ... position on Y-axis (0...1)
angle .. ratation angle (0...360)
xpeed, yspeed, rspeed, maccel, raccel ... speed and acceleration values

Source Code:
------------
The TuioClient Plugin comes with its full source code which can be
built using XCode 3.0 or later on Mac OS X 10.5 Leopard.

License:
--------
This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA

