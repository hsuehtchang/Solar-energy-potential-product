Files:
	Readme.txt: 	a guide to the use of this dataset.
	Locations.png:	locations of 10 cities in China.

Folders:
	Beijing
	Chongqing
	Guangzhou
	Harbin
	Kunming
	Lhasa
	Nanjing
	Shanghai
	Urumqi
	Xi'an

Under the folders:
	Shapefile: each polygon records information on a building in the city.
	

Attribute fields of the shapefile:
	ID:		(Long)		a unique number
	N_floor:	(Int)		number of floors
	A_roof: 	(Double)	area of building roof (m^2)
	A_facade: 	(Double)	area of building facades (m^2)
	Y_roof: 	(Double)	yearly solar irradation recieved by building roof (kWh/year)
	Y_facade:	(Double)	yearly solar irradation recieved by building facades (kWh/year)
	Y_total: 	(Double)	yearly solar irradation recieved by building roof and facades (kWh/year)
	

Instructions:
	A_roof = Shape_Area
	A_facade = Shape_Lengths ¡Á N_floor ¡Á 3
	Y_total = Y_roof + Y_facade