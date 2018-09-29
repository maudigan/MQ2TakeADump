MQ2TakeADump.dll: MacroQuest2's extension DLL for EverQuest
Copyright (C) 2018 Maudigan

This program is free software; you can redistribute it and/or modify it under the terms of
the GNU General Public License, version 2, as published by the Free Software Foundation.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
See the GNU General Public License for more details.
	
	
	▄▄▄█████▓ ▄▄▄       ██ ▄█▀▓█████     ▄▄▄         ▓█████▄  █    ██  ███▄ ▄███▓ ██▓███
	▓  ██▒ ▓▒▒████▄     ██▄█▒ ▓█   ▀    ▒████▄       ▒██▀ ██▌ ██  ▓██▒▓██▒▀█▀ ██▒▓██░  ██▒
	▒ ▓██░ ▒░▒██  ▀█▄  ▓███▄░ ▒███      ▒██  ▀█▄     ░██   █▌▓██  ▒██░▓██    ▓██░▓██░ ██▓▒	
	░ ▓██▓ ░ ░██▄▄▄▄██ ▓██ █▄ ▒▓█  ▄    ░██▄▄▄▄██    ░▓█▄   ▌▓▓█  ░██░▒██    ▒██ ▒██▄█▓▒ ▒
	▒██▒ ░  ▓█   ▓██▒▒██▒ █▄░▒████▒    ▓█   ▓██▒   ░▒████▓ ▒▒█████▓ ▒██▒   ░██▒▒██▒ ░  ░
	▒ ░░    ▒▒   ▓▒█░▒ ▒▒ ▓▒░░ ▒░ ░    ▒▒   ▓▒█░    ▒▒▓  ▒ ░▒▓▒ ▒ ▒ ░ ▒░   ░  ░▒▓▒░ ░  ░
	░      ▒   ▒▒ ░░ ░▒ ▒░ ░ ░  ░     ▒   ▒▒ ░    ░ ▒  ▒ ░░▒░ ░ ░ ░  ░      ░░▒ ░
	░        ░   ▒   ░ ░░ ░    ░        ░   ▒       ░ ░  ░  ░░░ ░ ░ ░      ░   ░░
	░  ░░  ░      ░  ░         ░  ░      ░       ░            ░
	░
	

DESCRIPTION:
-----------------------------------------------------------------------------------------
This plugin will allow you to dump EQ information out to CSV files, such as doors,
groundspawns, objects, NPCs, current zone and zonepoints. To take a dump use the
/takeadump command. You can optionally send a parameter to limit the dump to just
the specific data you are after, e.g. "/takeadump door". For the list of parameters
try "/takeadump help".

When run it will drop all the varios data dumps as CSV files in the macroquest
directory with the zone name, type, and timestamp in the filename.

The first row of the CSV is a description of the field (taken from the MQ objects).
The second row is a description of the datatype. Numeric and float data shows up as
plain numbers, boolean show up as true or false literals, and strings show up
as text surrounded by double quotes (the quotes may not display in excel but they will
in notepad).

"/takedump target" is a special case. If you use this you have to have a target. It
will dump that targets coordinates until it dies, you zone or you lose the target.
One row will dump out every time your targets heading changes.
