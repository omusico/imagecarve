Program takes a PGM image (assumed to be 8-bit) and outputs a G-code program that carves that image on a suitable CNC milling or routing machine.

It does enough trivial geometry to ensure that the tool doesn't cut into the desired surface, so it's able to generate a fine cut to follow a coarse cut.

It also somewhat optimizes the G-code, merging multiple steps along a line into a single command.