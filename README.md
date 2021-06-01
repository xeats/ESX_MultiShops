# esx_multishops

This must replace esx_shops, not launched with it.
Works just like esx_shops, with the same database table :

```SQL
INSERT INTO `shops` (store, item, price) VALUES
	('TwentyFourSeven','bread',30),
	('TwentyFourSeven','water',15),
	('RobsLiquor','bread',30),
	('RobsLiquor','water',15),
	('LTDgasoline','bread',30),
	('LTDgasoline','water',15),
	('myshopname','myitem',10)
;
```


Just modify/add these sections in config file :

``` lua
	RobsLiquor = { --name to use in DB
		Items = {},
		Type = 93, -- blip type (https://docs.fivem.net/docs/game-references/blips/)
		BlipColor = 27, -- blip color (https://docs.fivem.net/docs/game-references/blips/#blip-colors)
		MarkerType = 1, -- (https://docs.fivem.net/docs/game-references/markers/)
		MarkerColor = {r = 0, g = 128, b = 255}, -- RGB color (see https://www.w3schools.com/colors/colors_picker.asp)
		Name = "robs", -- name used for the blip (on the map)
		Pos = {
			vector3(1135.8, -982.2, 45.4),
			vector3(-1222.9, -906.9, 11.3),
			vector3(-1487.5, -379.1, 39.1),
			vector3(-2968.2, 390.9, 14.0),
			vector3(1166.0, 2708.9, 37.1),
			vector3(1392.5, 3604.6,  33.9),
			vector3(127.8,  -1284.7, 28.2), --StripClub
			vector3(-1393.4, -606.6, 29.3), --Tequila la
			vector3(-559.9, 287.0, 81.1) --Bahamamas
	}},
```


***Custom version of esx_shops to allow you customize markers, blips and names per store type***

# Legal
### License
esx_shops - shoppin'

Copyright (C) 2015-2020 Jérémie N'gadi

This program Is free software: you can redistribute it And/Or modify it under the terms Of the GNU General Public License As published by the Free Software Foundation, either version 3 Of the License, Or (at your option) any later version.

This program Is distributed In the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty Of MERCHANTABILITY Or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License For more details.

You should have received a copy Of the GNU General Public License along with this program. If Not, see http://www.gnu.org/licenses/.
