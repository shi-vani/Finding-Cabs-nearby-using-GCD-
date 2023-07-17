# Finding-Cabs-nearby-using-GCD- C++
Given GPS co-ordinates(in degrees) of a person who needs a cab and co-ordinates of all the cabs in the city stored in a text file in JSON format, find the user-id and name of all the cab drivers available in 50 km proximity.
# Approach Used
Obtain latitude and longitude of each cab in string format along with their user-id and name from the JSON encoded input file.

Convert latitude and longitude of the cab present in string format to double.

Convert latitude and longitude of both, the user and the cab present in degrees to radians.

Calculate distance between the user’s location and the cab using Great Circle Distance formula.

If distance is found to be less than or equal to 50 kms then output the user- id and name of the cab driver to a new file else take no action.
# Procedure to run the program :
Save the code and the file customers.json in a same location.

Now, compile the code(using cmd : g++ file_name.cpp) and run it(using cmd : ./a.out /home/gfg/customers.json) with passing file name customers.json along with proper location(e.g. /home/gfg/customers.json).

A file named answers.json will be created on the same location where code and customers.json file is existing

# Great Circle Formula
The great circle formula is given as follows:

d = rcos-1[cos a cos b cos(x-y) + sin a sin b]

where, 

r depicts the earth’s radius, 

a and b depict the latitude 

while the longitudes are depicted by x and y.
