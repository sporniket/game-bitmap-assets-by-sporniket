# Flexible bricks

A brick is deemed "flexible" when it can have a width as large as wanted, starting from 1 unit up to the whole width of the playing field.

Thus each tileset allows to generate bricks with a width as large as wanted. 

To hint at which tile to use for which part of the brick, all the individual tile of each tileset follows the following naming scheme, using a bitset :  `{left_end}{right_end}`

* `{left_end}` : the bit is clear when the left end is opened.
* `{right_end}` : the bit is clear when the right end is opened.

e.g., for a given tileset : 

* `01.xpm` is the tile to use to display the right end of a given brick with a width strictly greater than one unit.
* `11.xpm` is the tile to use to display a brick with a width of exactly one unit.


