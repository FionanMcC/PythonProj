# PythonProj
// ireland_counties.geojson //
in this file wee are setting bounderies of the different county bourders of the republic of Ireland and plotting then on a mapp image of Ireland. the map is also interactive meaning that when the mouse cursor is hovered above each county the colour of the hovered county is changed/ higlighted. There is also a clickable feature that will trigger a window that will show the BER ratings and related data of the selected county.

// map_test.py //
This is test code that tests the functions of the "ireland_counties.geojson" file as if it was a constituancy map for an election. e.g merging the results with the geomatey of the map, if there is no data for a constituency make the area grey.

// pandas_lookup.py //
This file executes multiple functions. The first function converts numbers from the BER ratings to a grade e.g A1, A2, A3, B1 ect. Contains the filepath. Reads chunks 100000 lines of the BER file at a time (The file is quite large) then combines the chunks. Converts the BER ratings to numeric values. Creates masks for each county. Finds an average BER rating by getting the mean average. Then finally prints the average BER rating and the grade to the user.

// test.py //
This is a test file that sets a literal value to the variables WINDOW_W and WINDOW_H. Then creates a class "CountyMapApp" that loads the county shapes, generates a fixed name for you file, provides some example population data for some counties. "project" Converts the latatude and longitude's into pixel coordinates. "draw_map" draws each polygon for each county. "on_mouse_move" Highlights each county and shows tooltip when highlighted.

// UI.py // 
In this file is the user interface. It first creates the main application window lable widget and an entry widget that users can enter there name. Then there is a feature added for if there is no characters added there will be an error prompting the user to enter there name. When the user inputs there name they will be given a greeting "Hello <name entered by user!>". Then creates a widget button for greeting and for exit, which then starts the Tkinter event loop.